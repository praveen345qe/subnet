# metacrafters - ERC20 and Vault Contracts

## Overview

This repository contains two Solidity smart contracts: ERC20 and Vault. These contracts are designed to work together to create a basic token (ERC20) and a corresponding vault for managing deposits and withdrawals.

## ERC20 Token Contract

### Features
- Name: Metacrafters
- Symbol: mtr
- Decimals: 18
- Minting: Allows the owner to mint new tokens.
- Burning: Allows token holders to burn their tokens.

### Functions
1. **transfer**: Transfers tokens from the sender to a specified recipient.
2. **approve**: Allows the owner to approve a spender to spend a certain amount of tokens on behalf of the owner.
3. **transferFrom**: Allows a spender to transfer tokens from the owner's account to another account if approved.
4. **mint**: Allows the owner to mint new tokens.
5. **burn**: Allows token holders to burn a certain amount of their tokens.

### Deployment
The ERC20 contract is deployed on a Subnet, providing a basic implementation of an ERC20 token.

## Vault Contract

### Features
- Manages deposits and withdrawals of ERC20 tokens.
- Uses the ERC20 contract for token interactions.
- Automatically mints and burns shares to track deposited tokens.

### Functions
1. **deposit**: Allows users to deposit ERC20 tokens into the vault, minting shares in return.
2. **withdraw**: Allows users to withdraw ERC20 tokens from the vault, burning the corresponding shares.

### Deployment
The Vault contract is deployed on the same Subnet as the ERC20 contract, creating a decentralized system for managing token deposits and withdrawals.

## Usage

1. Deploy the ERC20 contract on the desired Subnet.
2. Deploy the Vault contract on the same Subnet, providing the ERC20 contract address during deployment.
3. Interact with the ERC20 token using standard ERC20 functions.
4. Deposit and withdraw tokens using the Vault contract, which automatically manages shares.

## License

Both contracts are licensed under the MIT License. See the individual contract files for more details.

## Author 

pravenn 

pp055319@gmail.com
