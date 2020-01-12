# Stary Notary DAPP

## Dependencies
* Truffle v5.1.8
* OpenZeppelin-Solidity v2.4.0

## Name, Symbol and Address

* Name: Balboa Token
* Symbol: BLT
* Contract Address: `0x8b3B009Cb2a5137aE7b7827815cDa1Bb565cB014`
* See the Token on Rinkeby Testnet [here](https://rinkeby.etherscan.io/token/0x8b3b009cb2a5137ae7b7827815cda1bb565cb014)
* See the Contract Address on Rinkeby Testnet [here](https://rinkeby.etherscan.io/address/0x8b3b009cb2a5137ae7b7827815cda1bb565cb014)

## Description
Creates a Balboa Token (BLT) contract that creates a notary service for stars.

The contract allows users to:

* Create a star
* Retrieve a star by ID
* Sell a star
* Transfer a star (donation)
* Exchange a star with someone else

Some of the functions have certain validations in place like requiring that:
* Seller of a star owns the star
* An address can send a star it owns to itself
* Buyer can't buy star that isn't for sale
* Buyer must have enough ether to cover the star's cost


