# Solidity Smart Contracts - Vault and ERC20

# Task Assignment
These contracts were developed as part of an assignment from Metacrafter. For more information about Metacrafter, visit their website here.

## Contracts Overview
### 1. Vault Contract
. The Vault contract manages the deposit and withdrawal of ERC20 tokens into a staking mechanism where deposited tokens are converted into "shares". These shares represent ownership in the deposited tokens and can be withdrawn back to the original token at a later time.

## Functions
. deposit(uint _amount): Allows users to deposit ERC20 tokens into the vault, converting them into shares.
. withdraw(uint _shares): Allows users to withdraw shares from the vault, converting them back into ERC20 tokens.

## Implementation Details
. Uses an interface (IERC20) to interact with the ERC20 token.
. Tracks total shares issued (totalSupply) and individual user balances (balanceOf).


### 2. ERC20 Contract
. The ERC20 contract is a basic implementation of the ERC20 token standard with additional minting and burning functionalities.

## Functions
. transfer(address recipient, uint amount): Transfers tokens from the sender to the recipient.
. approve(address spender, uint amount): Allows the spender to withdraw tokens from the sender’s account multiple times, up to the amount.
. transferFrom(address sender, address recipient, uint amount): Allows the spender to transfer tokens from the sender's account to another account.
. mint(uint amount): Mints new tokens and assigns them to the caller.
. burn(uint amount): Destroys tokens from the caller's account, reducing the total supply.

## Additional Details
. Name: Solidity by Example
. Symbol: SOLBYEX
. Decimals: 18
