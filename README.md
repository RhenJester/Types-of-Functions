# Types-of-Functions
ETH + AVAX PROOF: Intermediate EVM Course | Types of Functions - ETH + AVAX

This Solidity smart contract, named TypesOfFunctions, is an ERC-20 token with additional functionalities. It is designed to showcase different types of functions commonly used in Ethereum smart contracts.

## Features

1. **ERC-20 Token**: Inherits from the OpenZeppelin ERC20 standard, providing basic token functionalities.
2. **Ownership**: Utilizes the Ownable contract from OpenZeppelin, ensuring that certain functions can only be executed by the contract owner.
3. **Minting**: The contract owner can mint new tokens and distribute them to specified addresses.
4. **Transferring**: Overrides the ERC-20 `transfer` function to add custom logic or features.
5. **Burning**: Allows token holders to burn a specified amount of their tokens.

