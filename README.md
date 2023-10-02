# MyToken
This is a Solidity program that creates a basic token in order to understand the concept of building a token and able to perform transaction by giving a value from a sender. The purpose of this program is able to know the basic use of functions and conditional statements that can be applied in building a token. 
## Description
A straightforward cryptocurrency-like token can be created and managed on the Ethereum network using the "MyToken" smart contract. This token includes fundamental functions including minting (the creation of new tokens) and burning (the destruction of current tokens), as well as the ability to maintain track of the token balances for various Ethereum addresses.
## Getting Started
### Executing Program
Remix is an online Solidity IDE that you may use to run this application. To get started, go to https://remix.ethereum.org/.
When you are on the Remix website, click the "+" icon in the left sidebar to start a new file. The file should be saved with a.sol extension (such as MyToken.sol). The code below should be copied and pasted into the file:
https://github.com/fger1011/MyToken/blob/d3d49010a8826539932e5907d00c1cc1b28d1c70/MyToken.sol

Click the "Solidity Compiler" tab in the left-hand sidebar to compile the code. Click the "Compile MyToken.sol" button after making sure the "Compiler" option is selected to "0.8.18" (or another compatible version).

Using the "Deploy & Run Transactions" tab in the left-hand sidebar, you can deploy the contract after the code has been compiled. Click the "Deploy" button after selecting the "MyToken" contract from the drop-down menu.

Once the contract is deployed, you can interact with it by calling all the function by clicking drop down for mint function. You have to first copy the account address below the "Environment" and paste it as the first parameter followed with the value of your choice. That is also the same goes with burn function (address, value). Then press transact in order to execute the function afterwards start calling the totalSupply below the tokenName so you will see the result and value of the created token. 

## Authors
Metacrafter Franco

