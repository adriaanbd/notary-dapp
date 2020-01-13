# Stary Notary DAPP

## Dependencies

### Project root dependencies

* Truffle v5.1.8
* OpenZeppelin-Solidity v2.4.0

### App dependencies

* Webpack and friends
* Web3

### Service dependencies

* Metamask browser extension with an account
* Rinkeby test ethers
* Infura free account and key

## Getting started

To get set up, please run the following commands:
1. Install dependencies: `$ npm install`
2. Compile contracts: `$ truffle compile`

### Locally

3. Run the backend with truffle development server: `$ truffle develop`
4. Install app apendencies and run the front-end with webpack: `$ cd app ; npm install ; npm run dev`
5. Open localhost on port `8080`, click [here](http://localhost:8080).
6. If Metamask is installed as an extension, please accept the prompt to connect your Account to StarNotary DAPP. Please switch to a custom RPC test network using the above-mentioned link on port `8080`. You'll need to import a key, so please copy the first private key that is in the output of Truffle develop, mine is: `a13f407ae1cb57e9a4887a5d2a3113d8510a3a92913aff63df9d6e28eca8c56c`, but yours might be different.

### Rinkeby


Make sure you've installed dependencies at the root directory of your project with `$ npm install`, and that you've compiled your contracts with `$ truffle compile`, as indicated in Getting Started.

To run this on the test network, you'd need an Infura account, which you can get over [here](https://infura.io/), for free in order to be able to connect to the Ethereum blockchain for read/write operations.

The app needs the following to files to be present in your root directory:
1. In your account, please look for your Infura key and paste it in a file called `.infura-key`.
2. In your Metamask account, please go to your settings and paste the private key seed of your account in a file called `.secret`.
3. Install app apendencies and run the front-end with webpack: `$ cd app ; npm install ; npm run dev`
4. Open localhost on port `8080`, click [here](http://localhost:8080).
5. If Metamask is installed as an extension, please accept the prompt to connect your Account to StarNotary DAPP, and make sure you are connected to the Rinkeby test network.
6. Now you can create a star and look up a star from the front end.

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


