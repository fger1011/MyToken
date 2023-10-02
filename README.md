# MyToken
This is a Solidity program that creates a basic token in order to understand the concept of building a token and able to perform transaction by giving a value from a sender. The purpose of this program is able to know the basic use of functions and conditional statements that can be applied in building a token. 
## Description
A straightforward cryptocurrency-like token can be created and managed on the Ethereum network using the "MyToken" smart contract. This token includes fundamental functions including minting (the creation of new tokens) and burning (the destruction of current tokens), as well as the ability to maintain track of the token balances for various Ethereum addresses.
## Getting Started
### Executing Program
Remix is an online Solidity IDE that you may use to run this application. To get started, go to https://remix.ethereum.org/.
When you are on the Remix website, click the "+" icon in the left sidebar to start a new file. The file should be saved with a.sol extension (such as MyToken.sol). The code below should be copied and pasted into the file:

// SPDX-License-Identifier: MIT
pragma solidity 0.8.18;

/*
       REQUIREMENTS
    1. Your contract will have public variables that store the details about your coin (Token Name, Token Abbrv., Total Supply)
    2. Your contract will have a mapping of addresses to balances (address => uint)
    3. You will have a mint function that takes two parameters: an address and a value. 
       The function then increases the total supply by that number and increases the balance 
       of the “sender” address by that amount
    4. Your contract will have a burn function, which works the opposite of the mint function, as it will destroy tokens. 
       It will take an address and value just like the mint functions. It will then deduct the value from the total supply 
       and from the balance of the “sender”.
    5. Lastly, your burn function should have conditionals to make sure the balance of "sender" is greater than or equal 
       to the amount that is supposed to be burned.
*/

contract MyToken {

    // public variables here\
    string public tokenName = "META";
    string public tokenAbbrv = "MTA";
    uint public totalSupply = 0;


    // mapping variable here
    mapping(address => uint) public balances;


    // mint function
    function mint (address _address, uint _value) public {
        totalSupply += _value;
        balances[_address] += _value;

    }
    // burn function
    function burn (address _address, uint _value) public {
        if(balances[_address] >= _value){
        totalSupply -= _value;
        balances[_address] -= _value;
        }
    }

}
Click the "Solidity Compiler" tab in the left-hand sidebar to compile the code. Click the "Compile MyToken.sol" button after making sure the "Compiler" option is selected to "0.8.18" (or another compatible version).

Using the "Deploy & Run Transactions" tab in the left-hand sidebar, you can deploy the contract after the code has been compiled. Click the "Deploy" button after selecting the "MyToken" contract from the drop-down menu.

Once the contract is deployed, you can interact with it by calling all the function by clicking drop down for mint function. You have to first copy the account address below the "Environment" and paste it as the first parameter followed with the value of your choice. That is also the same goes with burn function (address, value). Then press transact in order to execute the function afterwards start calling the totalSupply below the tokenName so you will see the result and value of the created token. 

## Authors
Metacrafter Franco

