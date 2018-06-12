
## how to contral smart contract with MEW  ( Withdraw Tokens and Eth etc.  

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

