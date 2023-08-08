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

## License

Please replace this section with the appropriate license information for your project.
