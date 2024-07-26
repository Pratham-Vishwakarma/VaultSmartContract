# The Vault Smart Contract

## Overview

The `the_vault` smart contract manages a token vault on the Aptos blockchain. It allows for the deposit, allocation, claim, and withdrawal of tokens. The contract tracks the total balance, total allocated amount, and specific allocations for addresses.

## Features

- **Deposit Tokens:** Admins can deposit tokens into the vault.
- **Allocate Tokens:** Admins can allocate tokens to specified addresses.
- **Claim Tokens:** Users can claim their allocated tokens.
- **Withdraw Tokens:** Admins can withdraw tokens from the vault.
- **View Functions:** Provides information on balance, total allocated amount, and specific allocations.

## Events

- **Tokens Deposited:** Triggered when tokens are deposited into the vault.
- **Allocation Made:** Triggered when tokens are allocated to an address.
- **Allocation Claimed:** Triggered when an address claims its tokens.
- **Tokens Withdrawn:** Triggered when tokens are withdrawn from the vault.

## Functions

### `deposit_tokens(admin: &signer, vault_address: address, amount: u64)`

Deposits tokens into the vault.

### `allocate_tokens(admin: &signer, vault_address: address, address: address, amount: u64)`

Allocates tokens to a specified address.

### `claim_tokens(account: &signer, vault_address: address)`

Allows a user to claim their allocated tokens.

### `withdraw_tokens(admin: &signer, vault_address: address, amount: u64)`

Withdraws tokens from the vault.

### `get_balance(vault_address: address): u64`

Returns the total balance of the vault.

### `get_total_allocated(vault_address: address): u64`

Returns the total amount allocated from the vault.

### `get_allocation(vault_address: address, addr: address): u64`

Returns the amount allocated to a specific address.

## Installation

1. Ensure you have the Aptos framework installed.
2. Deploy the contract using your Aptos development tools.

## Usage

1. **Deploy** the contract to the Aptos blockchain.
2. **Interact** with the contract using Aptos tools or SDKs.

## License

This project is licensed under the [MIT License](LICENSE).

## Contact

For questions or issues, please contact [pratham.vishwakarma125940@gmail.com](mailto:pratham.vishwakarma125940@gmail.com).
