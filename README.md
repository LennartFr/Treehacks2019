# Hyperledger Fabric and IBM Blockchain at TreeHacks 2019

# Repo URL: https://ibm.biz/TreeHacks2019

<img src="https://farm5.staticflickr.com/4503/37148677233_71edc5a37b_o.png" width="1041" height="53" alt="blueband">

## <a href="https://developer.ibm.com/code-and-response/">Code and Response initiative</a>

# Reuse Use Cases and Code Patterns:

## [IBM Bockchain Use Cases](https://www.ibm.com/blockchain/use-cases/)

## <a href="https://developer.ibm.com/code-and-response/technologies/blockchain">Blockchain Code Patterns for Code and Response</a>

## [All IBM Code Patterns for Blockchain](https://developer.ibm.com/patterns/category/blockchain)

# Dev Tool:

## [Visual Studio Code](https://code.visualstudio.com)
## [IBM Blockchain Platform in Visual Studio Marketplace](https://marketplace.visualstudio.com/items?itemName=IBMBlockchain.ibm-blockchain-platform)

# Step by step sample apps to quickly get up and running 

## Write Smart Contracts in NodeJS.

~~~~
 'use strict';
 const { Contract } = require('fabric-contract-api'); class MyContract extends Contract {
 //update ledger with a greeting to show that the function was called
 async instantiate(ctx) {
 let greeting = { text: 'Instantiate was called!' };
 await ctx.stub.putState('GREETING', Buffer.from(JSON.stringify(greeting)));
}
//take argument and create a greeting object to be updated to the ledger
 async transaction1(ctx, arg1) {
 console.info('transaction1', arg1);
 let greeting = { text: arg1 };
 await ctx.stub.putState('GREETING', Buffer.from(JSON.stringify(greeting)));
 return JSON.stringify(greeting);
 }
}   
module.exports = MyContract;
~~~~
https://www.hyperledger.org/blog/2018/10/26/hyperledger-fabric-now-supports-ethereum

<hr size="6">

### Hyperledger Fabric now supports Ethereum Virtual Machine (EVM) bytecode smart contracts. 
### Contracts can now be written in languages such as Solidity or Vyper. Along with introducing 
### a new smart contract runtime, Fabric also has a corresponding web3 provider which can be used 
### to develop decentralized applications (DApps) using web3.js.

<hr size="6">

## Demo: [The Blockchain Bean Supply Chain](https://www.ibm.com/thought-leadership/blockchainbean/)
## [Prerequisites](https://hyperledger-fabric.readthedocs.io/en/release-1.4/prereqs.html#prerequisites)
## Exercise 1: [Develop a Node.js smart contract and web app for a Global Finance with blockchain use case](https://developer.ibm.com/patterns/global-financing-use-case-for-blockchain/)
## Exercise 2: [Use IBM Blockchain Platform extension in VSCode to develop a Smart Contract](https://github.com/horeaporutiu/VSCodeTutorialBlockchain#use-ibm-blockchain-platform-extension-in-vscode-to-develop-a-smart-contract)  
## Exercise 3: [How to quickly connect a Smart Contract to IBM Blockchain Platform Starter Plan using VSCode](https://github.com/horeaporutiu/VSCodeRemoteNetwork#vscoderemotenetwork) 
## Exercise 4: [Run a commercial paper smart contract with the IBM Blockchain VSCode extension](https://developer.ibm.com/tutorials/run-commercial-paper-smart-contract-with-ibm-blockchain-vscode-extension/)
## [IBM Blockchain Platform](https://www.ibm.com/blockchain/platform)
