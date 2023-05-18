
# MyToken Contract
This is a smart contract written in Solidity, a programming language used for developing decentralized applications on the Ethereum blockchain. The contract represents a simple token called "MyToken" with the following features:

# Contract Details
SPDX-License-Identifier: MIT: This contract is licensed under the MIT license.
Solidity Version: This contract is written in Solidity version 0.8.18.
Public Variables
The contract defines the following public variables:

tokenName: A string variable representing the name of the token. In this case, it is set to "Prachi".
tokenAbbrv: A string variable representing the abbreviated name of the token. In this case, it is set to "PRA".
totalSupply: An unsigned integer variable representing the total supply of the token. It is initialized to 0.

# Mapping Variable
The contract defines the following mapping variable:

balances: A mapping that associates Ethereum addresses with their corresponding token balances. It maps addresses to unsigned integers representing the token balance of each address.

# Mint Function
The contract includes a mint function, which allows the creation of new tokens and assigns them to a specific address. The function takes two parameters:

_address: The Ethereum address to which the tokens will be assigned.
_value: The number of tokens to be minted and assigned.
When the mint function is called, it increases the total supply of the token by the specified value (_value) and updates the balance of the specified address (_address) by adding the minted tokens to it.

# Burn Function
The contract includes a burn function, which allows the destruction of existing tokens held by a specific address. The function takes two parameters:

_address: The Ethereum address from which the tokens will be burned.
_value: The number of tokens to be burned.
Before burning the tokens, the function checks if the specified address has a sufficient balance to burn the requested number of tokens. If the balance is sufficient, it decreases the total supply by the specified value (_value) and updates the balance of the specified address by subtracting the burned tokens from it.

Please note that both the mint and burn functions are public, meaning anyone can call them.

Note: This readme assumes you have a basic understanding of Ethereum and Solidity programming.
