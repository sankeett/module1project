# module1project

# Exception Handling Smart Contract

This is a Solidity smart contract that demonstrates the usage of exception handling mechanisms including `require()`, `assert()`, and `revert()`.

## Contract Overview

The `ExceptionHandlingContract` is a basic contract that manages a token-like system. It maintains an internal `totalSupply` variable and a `balances` mapping to track the balances of different addresses. The contract allows users to transfer tokens to other addresses.

## Functions

### `constructor(uint initialSupply)`

The constructor initializes the `totalSupply` and assigns the entire supply to the contract deployer's address.

### `transfer(address recipient, uint amount)`

This function allows users to transfer tokens from their account to a specified recipient. It checks if the given `amount` is greater than zero and if the sender has sufficient balance using the `require()` statement. If the conditions are met, the transfer is performed successfully.

### `assertExample(uint a, uint b)`

This function demonstrates the usage of the `assert()` statement. It performs a division operation and asserts that the divisor (`b`) is not zero. If the condition is not met, the transaction will revert.

### `revertExample()`

This function demonstrates the usage of the `revert()` statement. It always reverts the transaction with a custom revert message.

## Testing

To test the contract, you can deploy it on a compatible Ethereum development network and interact with it using a compatible Ethereum wallet or development framework.



