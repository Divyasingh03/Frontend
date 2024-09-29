# Contract Details
## Greeter.sol
The contract is defined with the name "Greeter" and specifies that it complies with the MIT license.
The contract contains a private string variable called "greeting," which will store the greeting message added by users. The "private" visibility modifier restricts direct access to this variable from outside the contract.
The setGreeter function allows users to add a new message to the "greeter" string. It takes a string parameter _name and appends it to the end of the array.
The deposit function is a function to deposit tokens to our contract.

# Client
It is a react frontend app that uses bootstrap library for css of components. We have also used react useEffect as well as use State hooks to handle components state on thier mounting on the webpage.

# Setup
## Use the following steps to deploy the DAPP
### Step1: Clone the repository
### Step2: open three terminals in vs code and in first terminal run ``cd ./client`` the run ``npm i``
### Step1: in second terminal run `` cd ./contract`` then run ```npm i``` then ```npx hardhat node```
### Step1: in third terminal run `` cd ./contract`` then run ```npx hardhat --network localhost run scripts/sample-script.js```
### Step1: in first terminal again run ``npm run start``
