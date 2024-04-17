# Solidity Error Handling Example

This repository demonstrates the use of various error handling techniques in Solidity, including `require`, `revert`, `assert`, and custom error definitions. The purpose is to provide a practical guide for developers new to blockchain and smart contract development, highlighting how to manage exceptions and errors in their code effectively.

# Description

The Solidity Error Handling Example includes a set of functions designed to showcase different ways to handle errors and unexpected inputs in a smart contract. The contract includes:
- Validations using `require` that ensure inputs meet certain conditions before proceeding.
- Use of `revert` to undo all changes when conditions are not met.
- `assert` to check for invariants within the contract.
- Custom errors for more detailed and specific error handling. 

These functionalities are crucial for maintaining the integrity and security of a smart contract on the Ethereum blockchain.

## Functions

### 1. `doubleIfGreaterThanTen(uint number)`
Doubles the input if it is greater than 10.
- **Parameters:**
  - `number`: Unsigned integer to be doubled if it meets the condition.
- **Returns:** The doubled value of `number` if it is greater than 10.
- **Error Handling:** Uses `require` to ensure the function only processes numbers greater than 10, reverting with an error message otherwise.

### 2. `doubleAndCheck(uint input)`
Doubles a state variable `currentMultiplier` and checks that the input is not greater than 10.
- **Parameters:**
  - `input`: Unsigned integer to check against the condition.
- **Returns:** The new value of `currentMultiplier` after being doubled.
- **Error Handling:** Uses `revert` to undo all changes if `input` is greater than 10, providing a message that the input should not exceed this value.

### 3. `squareAndAssertZero(uint input)`
Squares the `currentMultiplier` and asserts that the input is zero.
- **Parameters:**
  - `input`: Unsigned integer expected to be zero.
- **Returns:** A string message "Input matches zero" if the assertion passes.
- **Error Handling:** Utilizes `assert` to check for the condition that `input` must be zero, primarily used here to ensure that there are no errors in the internal state of the contract.

# License

This contract is provided under the MIT License (SPDX-License-Identifier: MIT), which allows for the use, modification, and distribution of the code with certain restrictions. Users of this contract should review and comply with the terms of the MIT License.
 For any queries :
 rahullunthi99@gmail.com
