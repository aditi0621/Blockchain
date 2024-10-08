# Javascript hashing and Solidity Smart Contract Assignment

## Overview

This folder contains a collection of simple Solidity smart contracts that demonstrate various basic functionalities. Each contract is designed to address a specific task, such as storing data, counting, or implementing voting mechanisms. The contracts are well-documented with comments explaining their functionality.

## Folder Structure

- **Assignment**
  - [`q1.js`](q1.js): SHA-256 Hash with Specific Prefix
  - [`q2.js`](q2.js) SHA-256 Hash with Specific Starting String
  - [`q3.js`](q3.js): Finding a Nonce for a Given Input
  - [`q4.png`](q4.png): Making the Zombie Factory
  - [`q5.sol`](q5.sol): Donation Smart Contract

### 1. **SHA-256 Hash with Specific Prefix ([`q1.js`](q1.js))**

- Finds an input string that outputs a SHA-256 hash starting with a specified prefix.

### 2. **SHA-256 Hash with Specific Starting String ([`q2.js`](q2.js))**

- Finds a hash that starts with a specified prefix and the input string starts with a given string.

### 3. **Finding a Nonce for a Given Input ([`q3.js`](q3.js))**

- Finds a nonce for a given input string such that the resulting SHA-256 hash starts with a specified prefix.

### 4. **Making the Zombie Factory ([`q4.png`](q4.png))**

- Making the Zombie Factory At cryptoZombies. [`q4.png`](q4.png)

### 5. **Donation Smart Contract ([`q5.sol`](q5.sol))**

- Allows individuals to donate Ether to the contract and the owner to transfer the collected donations to various recipients.

## Usage

1. **Compilation**: Use the Solidity compiler (`solc`) or an online IDE like Remix to compile the contracts.
2. **Deployment**: Deploy the contracts on an Ethereum test network (e.g., Ropsten, Rinkeby) or a local Ethereum network like Ganache.
3. **Interaction**: After deployment, interact with the contracts via a web3 interface, like Remix or using web3.js/ethers.js in a dApp.
