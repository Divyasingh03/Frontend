# Contract Details
## Greeter.sol
The contract is defined with the name "Greeter" and specifies that it complies with the MIT license.

The contract contains a private string variable called "greeting," which will store the greeting message added by users. The "private" visibility modifier restricts direct access to this variable from outside the contract.

The setGreeter function allows users to add a new message to the "greeter" string. It takes a string parameter _name and appends it to the end of the array.

The deposit function is a function to deposit tokens to our contract.

# Client
It is a react frontend app that uses bootstrap library for css of components. We have also used react useEffect as well as use State hooks to handle components state on thier mounting on the webpage.

# Code
~~~
//SPDX-License-Identifier: Unlicense
pragma solidity ^0.8.0;

import "hardhat/console.sol";

contract Greeter {
    string private greeting;

    constructor(string memory _greeting) {
        console.log("Deploying a Greeter with greeting:", _greeting);
        greeting = _greeting;
    }

    function greet() public view returns (string memory) {
        return greeting;
    }

    function setGreeting(string memory _greeting) public {
        console.log("Changing greeting from '%s' to '%s'", greeting, _greeting);
        greeting = _greeting;
    }

    function deposit() public payable {}

}
~~~
# Setup
## Use the following steps to deploy the DAPP
### Step1: Clone the repository
### Step2: Open three terminals in vs code and in first terminal run ``cd ./client`` the run ``npm i``
### Step1: In second terminal run `` cd ./contract`` then run ```npm i``` then ```npx hardhat node```
### Step1: In third terminal run `` cd ./contract`` then run ```npx hardhat --network localhost run scripts/sample-script.js```
### Step1: In first terminal again run ``npm run start``

# Author
Divya Singh
