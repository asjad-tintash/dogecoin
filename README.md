### Setting up dogecoin node

Used this link to setup the dogecoin node
https://github.com/dogecoin/dogecoin/blob/master/doc/build-unix.md

Faced an error related to atomic compare exchange, fixed it by following steps in this video
https://www.youtube.com/watch?v=2_EDhIvI7H8


### Starting the node
Used the command 
```./dogecoind -daemon -testnet``` to start testnet node

Executing commands

### Syncing data: <br/>
Command:  
```
./dogecoind -printtoconsole -testnet
```
Output:

```Prints a lot of data on console```


### Get Address: <br />

Used this command to create new wallet <br />

```./dogecoin-cli getnewaddress "asjad-wallet"```

Command:


```./dogecoin-cli getaddressesbyaccount "asjad-wallet"```

Output:
```
[
  "nhzyi8jnm5wEBPy14wsvmkCBSWnoSVQUWD", 
  "nqrGMFjKXtoGV2L8txToL7wMBJLCVRWZvY"
]
```

### Get Account Balance:
Command:
```/dogecoin-cli getbalance "asjad-wallet" ``` <br /> 
Output:
```0.00000000```

### Create Account in Wallet

### Create Raw Transaction
Command:
```
./dogecoin-cli createrawtransaction "[{\"txid\":\"61736a7361646e6a736b6b6e6473666b6e646b6e6b736e64666a6e63646a6973\",\"vout\":0}]" "{\"address\":\"nhzyi8jnm5wEBPy14wsvmkCBSWnoSVQUWD\"}"
```

Output:
```
error code: -5
error message:
Invalid Dogecoin address: address
```


### Get Public Key / Private Key / Address
#### Private Key
```
./dogecoin-cli dumpprivkey nqrGMFjKXtoGV2L8txToL7wMBJLCVRWZvY
```

Output
```
cjjFKW9r8DbrmcJqL3e41R71RACZWy7fFDcq9CUEEEZ9NJY3bQcC
```


### Create Transaction
```
./dogecoin-cli createrawtransaction "[{\"txid\":\"49ffda766599405bb5b3020b8821fddefed9fc1ff016a42310bbebfd72567664\",\"vout\":0}]" "{\"nrGYZuFu5hesbobSX1jJmHWAKe6LJBJR6B\":30}" 
```

Output:
```
010000000164765672fdebbb1023a416f01ffcd9fedefd21880b02b3b55b40996576daff490000000000ffffffff01005ed0b2000000001976a914f2270cacccb703be695faf3ebd5403ea2b2fb69588ac00000000
```


### Send Transaction
```
./dogecoin-cli sendrawtransaction 010000000164765672fdebbb1023a416f01ffcd9fedefd21880b02b3b55b40996576daff49000000006b4830450221008adfe96352bc3c791c60e8e0324d938d361488c06d23150786f006637ece7cd4022074d3733179f4413366f704452b784ce020e77df811578c2eacb93f23e811785d012102bbfe069b161a6ab543d018bda73953686d111a2c15df1c6ccb2f5cc2a85fc715ffffffff01005ed0b2000000001976a914f2270cacccb703be695faf3ebd5403ea2b2fb69588ac00000000
```

Output:
```
e4d68a41fa3511743ef9d440b8f12abd9466c265b50a4343fa5c2fd9a067be33
```












