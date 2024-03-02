# Types-of-Functions
ETH + AVAX PROOF: Intermediate EVM Course | Types of Functions - ETH + AVAX

This Solidity smart contract, named TypesOfFunctions, is an ERC-20 token with additional functionalities. It is designed to showcase different types of functions commonly used in Ethereum smart contracts.

## Table of Contents
- [Features](#features)
- [Prerequisites](#prerequisites)
- [Installation](#installation)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)

## Features

1. **ERC-20 Token**: Inherits from the OpenZeppelin ERC20 standard, providing basic token functionalities.
2. **Ownership**: Utilizes the Ownable contract from OpenZeppelin, ensuring that certain functions can only be executed by the contract owner.
3. **Minting**: The contract owner can mint new tokens and distribute them to specified addresses.
4. **Transferring**: Overrides the ERC-20 `transfer` function to add custom logic or features.
5. **Burning**: Allows token holders to burn a specified amount of their tokens.

## Prerequisites

Make sure you have the following tools installed:

- [Node.js](https://nodejs.org/)
- [npm](https://www.npmjs.com/) (Node Package Manager)
- [Truffle](https://www.trufflesuite.com/truffle)
- [Ganache](https://www.trufflesuite.com/ganache) (for local development)

## Installation

1. Clone the repository:

```bash
git clone https://github.com/your-username/TypesOfFunctions.git
cd TypesOfFunctions
```

2. Install dependencies:

```bash
npm install
```

## Usage

1. Deploy the contract locally for testing:

```bash
truffle migrate --reset --network development
```

2. Interact with the deployed contract using the Truffle console:

```bash
truffle console
```

3. Use the contract's functions:

```javascript
// Example: Minting new tokens
let tokenInstance = await TypesOfFunctions.deployed();
let recipientAddress = "0x1234567890123456789012345678901234567890";
let amountToMint = web3.utils.toWei("100", "ether");

await tokenInstance.mint(recipientAddress, amountToMint);
```
