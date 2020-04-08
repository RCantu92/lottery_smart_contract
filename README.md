# Decentralized Lottery

This project aims to provide a lottery smart contract that accepts Ether into its pot. The manager would then call the function that would randomly select a winner to whom the pot of Ether would be awarded to.

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. See deployment for notes on how to deploy the project on a live system.

### Installing

What things you need to install the software and how to install them

solc

```
npm install solc
```
Mocha

```
npm install --save mocha
```
Ganache CLI

```
npm install --save ganache-cli
```
web3

```
npm install --save web3@v.1.0.0-beta.35
```
truffle-hdwallet-provider

```
npm install truffle-hdwallet-provider
```
React

```
npm install --save react
```

You will also need to install [MetaMask](https://metamask.io/) on your browser, and create an account with [Infura](https://infura.io/).

## Running the tests

Navigate into the lottery-smart-contract/ directory, and once in there, run the
following in the command line:

```
npm run test
```
If all the tests are passed, you should an output similar to the following:

![](./images/npm_test_output.png)

*(Note: the warning should not appear and will be looked into further.)

## Deployment

To deploy the lottery smart contract onto the Rinkeby Ethereum testnet, you would navigate back to the lottery-smart-contract directory and run the following in the command line:

```
node deploy.js
```

Once deployed, you should see message like the following:

![](./images/node_deploy_output.png)

*(Note: the output is comprised of both the contract ABI and the contract address. Also, this is a different deployed address than the listed at the end of this README.)

To now render a local instance of contract on your browser, navigate to the lottery-react/ directory.

Once inside, run the following in the command line:

```
npm run start
```

After running the above command, the React app should launch in your browser. The following gif demonstrates the process of submitting funds to the lottery and selecting a winner.

![](./images/decentralized_lottery_demo.gif)

This contract is deployed on the rinkeby testnet under address [0x40102DAa67EE7c1748F01FB22578d778a0E55f25](https://rinkeby.etherscan.io/address/0x40102daa67ee7c1748f01fb22578d778a0e55f25).

## Built With

* [npm](https://www.npmjs.com/) - Package manager for the JavaScript programming language.
* [Solidity, v.4.17.0](https://solidity.readthedocs.io/en/v0.4.17/) - Smart Contract programming language used.
* [JavaScript](https://developer.mozilla.org/en-US/docs/Web/javascript) - Programming language used.
* [Path](https://nodejs.org/api/path.html) - Module that provides ability for working with file and directory paths.
* [File System](https://nodejs.org/api/fs.html) - Module that provides an API for interacting with the file system.
* [solc](https://github.com/ethereum/solc-js) - Module for compiling the Solidity programming language.
* [Mocha](https://mochajs.org/) - JavaScript test framework.
* [Ganache CLI](https://www.npmjs.com/package/ganache-cli) - the command line version of Ganache, your personal blockchain for Ethereum development.
* [web3](https://github.com/ethereum/web3.js/) - This is the Ethereum JavaScript API which connects to the Generic JSON-RPC spec. Used v.1.0.0-beta.35.
* [Assert](https://nodejs.org/api/assert.html) - Module that provides a set of assertion functions for verifying invariants.
* [Infura](https://infura.io/) - API used to access the Ethereum and IPFS networks.
* [truffle-hdwallet-provider](https://github.com/trufflesuite/truffle-hdwallet-provider) - HD Wallet-enabled Web3 provider. Used to sign transactions for addresses derived from a 12-word mnemonic.
* [React](https://reactjs.org/) - JavaScript library for building user interfaces.
* [Create React App](https://github.com/facebook/create-react-app) - Tool to build React apps.
* [MetaMask](https://metamask.io/) - Browser based wallet used to connect to the Ethereum mainnet as well as testnets.

## Authors

* **Roberto Cantu**  - [GitHub](https://github.com/RCantu92)