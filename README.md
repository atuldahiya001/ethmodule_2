# Smart Contract with Front-End Interaction

This Solidity smart contract provides a basic framework for managing funds and interacting with the contract's balance. It includes functions for depositing and withdrawing funds, as well as retrieving the contract's balance and displaying the wallet address associated with the contract.

## Contract Details

- **Solidity Version:** ^0.8.7
- **License:** UNLICENSED (Please replace with appropriate license information)

## Contract Functionality

### Constructor

The constructor initializes the contract with an initial balance and sets the wallet address of the deployer as the owner.

### Functions

1. **getBalance()**: This function is a view function that returns the current balance of the contract.

2. **DisplayAddress()**: This function emits the `showAddress` event, displaying the wallet address associated with the contract.

3. **Deposite(uint256 deposit_val)**: Allows users to deposit funds into the contract. The deposited amount is added to the contract's balance, and the `deposite` event is emitted.

4. **Withdraw(uint256 withdraw_val)**: Allows users to withdraw funds from the contract. It checks if the contract's balance is sufficient for the requested withdrawal amount. If the balance is sufficient, the withdrawal amount is deducted from the balance, and the `withdraw` event is emitted. If the balance is insufficient, a custom `insuficient_balance` error is thrown.

## Events

- **showAddress(address walAdress)**: Emitted when the `DisplayAddress` function is called to display the wallet address associated with the contract.

- **deposite(uint256 deposit_val, uint256 balance)**: Emitted when funds are deposited into the contract. It logs the deposited amount and the new contract balance.

- **withdraw(uint256 withdraw_val, uint256 balance)**: Emitted when funds are withdrawn from the contract. It logs the withdrawn amount and the new contract balance.

## Important Notes

- This code is intended for educational purposes and provides a basic example of a smart contract's functionality.
- The contract lacks proper access control mechanisms and does not include error handling for all scenarios.
- For production use, additional security measures, access controls, and error handling should be implemented.

- # React Wallet App with Smart Contract Interaction

This React application demonstrates wallet interactions with a smart contract on the Ethereum blockchain. It allows users to connect their MetaMask wallet, view account details, deposit and withdraw funds using a smart contract.

## Getting Started

1. Clone or download this repository to your local machine.

2. Open the project folder in your preferred code editor.

3. Install the required dependencies using npm or yarn:

   ```sh
   npm install
   # or
   yarn install

Certainly! Here's the content of the README file in markdown format as code:

markdown
Copy code
# React Wallet App with Smart Contract Interaction

This React application demonstrates wallet interactions with a smart contract on the Ethereum blockchain. It allows users to connect their MetaMask wallet, view account details, deposit and withdraw funds using a smart contract.

## Getting Started

1. Clone or download this repository to your local machine.

2. Open the project folder in your preferred code editor.

3. Install the required dependencies using npm or yarn:

4. Start the development server

5. Access the application in your web browser at http://localhost:3000.

# Features
Connect your MetaMask wallet to the application.
View your account details and current balance.
Deposit funds (5 ETH) into the smart contract.
Withdraw funds (5 ETH) from the smart contract.

# How to Use
Install the MetaMask extension in your browser.

Launch the application and click the "CONNECT TO THE METAMASK" button to connect your wallet.

Once connected, your account details and current balance will be displayed.

Use the "Deposite 5 ETH" button to deposit 5 ETH into the smart contract.

Use the "Withdraw 5 ETH" button to withdraw 5 ETH from the smart contract.

# Notes
This application interacts with a specific smart contract deployed at the contract address 0x5FbDB2315678afecb367f032d93F642f64180aa3. Ensure that the contract is deployed and accessible on the Ethereum network you are connected to.
Make sure your MetaMask wallet is connected to the correct network (e.g., Ropsten, Rinkeby, or Ethereum Mainnet) to interact with the deployed contract.

# Disclaimer
This application is for educational purposes and serves as an example of wallet interaction with Ethereum smart contracts.
Ensure that you understand the risks associated with using Ethereum and interacting with smart contracts.
Use test networks and small amounts of cryptocurrency for testing to avoid potential losses.
