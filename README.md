# T-Shirt Store Smart Contract

## Introduction

The T-Shirt Store smart contract is a Solidity-based Ethereum smart contract that facilitates the purchase of virtual T-Shirts using a custom ERC20 token named DEGEN. This contract allows users to redeem their DEGEN tokens for virtual T-Shirts of two different types: PUMA and US_POLO. 

## Features

- Users can mint DEGEN tokens to their address.
- Users can burn their DEGEN tokens to destroy them.
- Users can redeem DEGEN tokens for virtual T-Shirts.
- Two types of T-Shirts are available: PUMA and US_POLO.
- Users can transfer DEGEN tokens to other addresses.

## Dependencies

This contract uses OpenZeppelin contracts for ERC20 functionality and for the Ownable access control.

## Contract Details

### ERC20 Token

- The contract inherits from the ERC20 contract, providing standard token functionality such as transfer, minting, and burning.

### T-Shirt Store

- The T-Shirt Store contract extends ERC20 and Ownable contracts.
- Users can mint tokens to their address using the `mintTokens` function, which can only be called by the contract owner.
- Users can burn tokens using the `BurnTokens` function, destroying tokens from their balance.
- Users can redeem DEGEN tokens for T-Shirts using the `RedeemTShirt` function.
- T-Shirt purchase costs are predefined constants.
- The contract emits an event `TShirtPurchased` upon successful T-Shirt redemption.
- Users can transfer DEGEN tokens using the `transferTokens` function.
- The contract maintains a mapping of user addresses to their purchased T-Shirt type.
- The `getUserTShirtType` function allows users to retrieve their purchased T-Shirt type.

## Usage

1. Deploy the T-Shirt Store contract to an Ethereum network.
2. Mint DEGEN tokens to the desired addresses using the `mintTokens` function.
3. Users can burn their DEGEN tokens if needed using the `BurnTokens` function.
4. Users can redeem DEGEN tokens for T-Shirts using the `RedeemTShirt` function.
5. Users can transfer DEGEN tokens to other addresses using the `transferTokens` function.
6. Users can check their purchased T-Shirt type using the `getUserTShirtType` function.

## License

This code is released under the MIT License. See the provided `LICENSE` file for details.
