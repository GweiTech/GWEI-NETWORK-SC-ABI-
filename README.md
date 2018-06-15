
## How to Withdraw Tokens and Eth with MEW

#### 1. Open a wallet page that supports interactions with the contract, take mycrypto for example, open
 https://www.mycrypto.com/contracts/interact  
 
  
#### 2. Input ABI and Pool Address, click [Access] button  

----------------------------------------------------------------

#### Withdraw ETH (For contributor)
``` 
[
    {
      "constant": false,
      "inputs": [],
      "name": "withdrawAll",
      "outputs": [],
      "payable": false,
      "stateMutability": "nonpayable",
      "type": "function"
    }
]
``` 
check ![Withdraw function screenshot](https://github.com/GweiTech/GWEI-NETWORK-SC-ABI-/blob/master/Withdraw.jpg)


#### Pay ETH to fund (For creator)
``` 
[
    {
      "constant": false,
      "inputs": [
        {
          "name": "_presaleAddress",
          "type": "address"
        },
        {
          "name": "_minPoolBalance",
          "type": "uint256"
        },
        {
          "name": "_gasLimit",
          "type": "uint256"
        },
        {
          "name": "_data",
          "type": "bytes"
        }
      ],
      "name": "payToPresale",
      "outputs": [],
      "payable": false,
      "stateMutability": "nonpayable",
      "type": "function"
    }
]

``` 

check ![PayTofund function screenshot](https://github.com/GweiTech/GWEI-NETWORK-SC-ABI-/blob/master/PayToFound.jpg)

#### Get your tokens (For contributor, the token has been confirmed)
``` 
[
    {
      "constant": false,
      "inputs": [
        {
          "name": "tokenAddress",
          "type": "address"
        },
        {
          "name": "recipients",
          "type": "address[]"
        }
      ],
      "name": "transferTokensTo",
      "outputs": [],
      "payable": false,
      "stateMutability": "nonpayable",
      "type": "function"
    }
]
``` 
check ![GetTokens function screenshot](https://github.com/GweiTech/GWEI-NETWORK-SC-ABI-/blob/master/GetYourTokens.jpg)


#### Deposit (For contributor)
``` 
[
    {
      "constant": false,
      "inputs": [],
      "name": "deposit",
      "outputs": [],
      "payable": true,
      "stateMutability": "payable",
      "type": "function"
    }
]
``` 
check ![GetTokens function screenshot](https://github.com/GweiTech/How-to-Withdraw-Tokens-and-Eth-with-MEW/blob/master/deposit.jpg)





#### Confirm tokens (For creator, the fund has paid)
``` 
[
    {
      "constant": false,
      "inputs": [
        {
          "name": "tokenAddress",
          "type": "address"
        }
      ],
      "name": "confirmTokens",
      "outputs": [],
      "payable": false,
      "stateMutability": "nonpayable",
      "type": "function"
    }
]
``` 
check ![GetTokens function screenshot](https://github.com/GweiTech/How-to-Withdraw-Tokens-and-Eth-with-MEW/blob/master/ConfirmTokens.jpg)

#### Transfer tokens to all contributors (For creator, the token has been confirmed)
``` 
[
    {
      "constant": false,
      "inputs": [
        {
          "name": "tokenAddress",
          "type": "address"
        }
      ],
      "name": "transferTokensToAll",
      "outputs": [],
      "payable": false,
      "stateMutability": "nonpayable",
      "type": "function"
    }
]
``` 
check ![GetTokens function screenshot](https://github.com/GweiTech/How-to-Withdraw-Tokens-and-Eth-with-MEW/blob/master/TransferTokensToAllContributors.jpg)



#### Get pool status (For creator)
``` 
[
    {
      "constant": true,
      "inputs": [],
      "name": "getPoolstatus",
      "outputs": [
        {
          "name": "",
          "type": "uint8"
        },
        {
          "name": "",
          "type": "uint256"
        },
        {
          "name": "",
          "type": "uint256"
        },
        {
          "name": "",
          "type": "uint256"
        },
        {
          "name": "",
          "type": "address"
        },
        {
          "name": "",
          "type": "address"
        },
        {
          "name": "",
          "type": "address[]"
        },
        {
          "name": "",
          "type": "uint256[]"
        }
      ],
      "payable": false,
      "stateMutability": "view",
      "type": "function"
    }
]
``` 
check ![GetTokens function screenshot](https://github.com/GweiTech/How-to-Withdraw-Tokens-and-Eth-with-MEW/blob/master/GetPoolStatus1.jpg)




