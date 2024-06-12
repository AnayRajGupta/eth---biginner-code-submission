# Project  mudraBhandar

This Solidity program demonstrates a simple use of the language to create our own personal token using contracts in the Solidity programming language. The purpose of this program is to clarify the concepts for those who are new to Solidity and want to get a feel for how it works.


## Description

This program is a simple contract written in Solidity, a programming language used for developing smart contracts on the Ethereum blockchain. The contract has a few variables, a mapping and two functions that are used to mint and burn the tokens. It is a quite simple and straightforward program that can be very heplful for begineers to develop projects in future.

## Getting Started


### Executing program

To run this program, you can use Remix, an online Solidity IDE. To get started, go to the Remix website at https://remix.ethereum.org/.
Once you are on the Remix website, create a new file by clicking on the "+" icon in the left-hand sidebar. Save the file with a .sol extension (e.g., contractOne.sol). Copy and paste the following code into the file:
```javascript
// SPDX-License-Identifier: MIT
pragma solidity ^0.8.0;

contract mudraBhandaar {
    string public tokenName = "KUBER";
    string public tokenAbbrv = "KBR";

    uint public totalSupply = 0;

    mapping(address => uint) public balances;

    function mint(address _address, uint _value) public {
        totalSupply += _value;
        balances[_address] += _value;
    }

    function burn(address _address, uint _value) public {
        if (balances[_address] >= _value) {
            totalSupply -= _value;
            balances[_address] -= _value;
        }
    }
}

```
To compile the code, click on the "Solidity Compiler" tab in the left-hand sidebar. Make sure the "Compiler" option is set to "0.8.18" (or another compatible version), and then click on the "Compile contractOne.sol" button.

Once the code is compiled, you can deploy the contract by clicking on the "Deploy & Run Transactions" tab in the left-hand sidebar. Select the "contractOne" contract from the dropdown menu, and then click on the "Deploy" button.

Once the contract is deployed, you can interact with it using the functions creted tomint and burn the tokens. Also, we can see the updated values every time by accessing the value of "Token_Supply" variable. Further, we can mint token using the "mint" function and we can burn the tokens using the burn "function" by providing the values for the necessary parameters. The working of the programcan be very easily understood by studying the code as given above.
Once the contract is deployed, you can interact with it using the functions creted tomint and burn the tokens. Also, we can see the updated values every time by accessing the value of "Token_Supply" variable. Further, we can mint token using the "mint" function and we can burn the tokens using the burn "function" by providing the values for the necessary parameters. The working of the program can be very easily understood by studying the code as given above.

```

## Authors

Anay Raj Gupta
