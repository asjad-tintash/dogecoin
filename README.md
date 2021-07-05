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

Get Faucet


Create Transaction  / Send Transaction











