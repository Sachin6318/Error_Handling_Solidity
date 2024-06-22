# Implementation of the require(), assert() and revert() statements.

This Solidity program is a simple "Error handling" program that demonstrates the basic syntax and functionality of the error handling methods in the Solidity programming language. The purpose of this program is to serve as a starting point for those who are new to Errror handling in Solidity and want to get a feel for how it works.

## Description

This program is a simple contract written in Solidity, a programming language used for developing smart contracts on the Ethereum blockchain. The contract has three different functions for implementing require(), assert() and revert() statements in solidity. This program serves as a simple and straightforward introduction to Error Handling in Solidity programming, and can be used as a stepping stone for more complex projects in the future.

## Getting Started

Executing program
To run this program, you can use Remix, an online Solidity IDE. To get started, go to the Remix website at https://remix.ethereum.org/.

Once you are on the Remix website, create a new file by clicking on the "+" icon in the left-hand sidebar. Save the file with a .sol extension (e.g., HelloWorld.sol). Copy and paste the following code into the file:



       
        // SPDX-License-Identifier: MIT
           pragma solidity 0.8.18;

     contract Error {
        uint public i = 12;
        function testRequire(uint _i) public  {require(_i > 10, "Input must be greater than 10");
        i = i+10;

    }

    function testRevert(uint _i) public  {

        i=i+10;
        if (_i <= 10) {
            revert("Input must be greater than 10");
        }
    }


    function testAssert() public {

        assert(i >= 10);
        i=i+10;
    } 

}

To compile the code, click on the "Solidity Compiler" tab in the left-hand sidebar. Make sure the "Compiler" option is set to "0.8.18" (or another compatible version), and then click on the "Compile HelloWorld.sol" button.

Once the code is compiled, you can deploy the contract by clicking on the "Deploy & Run Transactions" tab in the left-hand sidebar. 
Once the contract is deployed, you can interact with it by calling the testrequire, testrevert, testassert functions.

## Authors

Sachin Singh
@Sachin17234
sachinsingh6318@gmail.com


## License

This project is licensed under the MIT License.
