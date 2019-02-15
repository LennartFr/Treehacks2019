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

Hyperledger Fabric now supports Ethereum Virtual Machine (EVM) bytecode smart contracts. 
Contracts can now be written in languages such as Solidity or Vyper. Along with introducing 
a new smart contract runtime, Fabric also has a corresponding web3 provider which can be used 
to develop decentralized applications (DApps) using web3.js.

### [EVM_Smart_Contracts tutorial](https://github.com/hyperledger/fabric-chaincode-evm/blob/master/examples/EVM_Smart_Contracts.mdz)

<hr size="6">

## Demo: [The Blockchain Bean Supply Chain](https://www.ibm.com/thought-leadership/blockchainbean/)
## [Prerequisites](https://hyperledger-fabric.readthedocs.io/en/release-1.4/prereqs.html#prerequisites)
## Tutorial 1: [Develop a Node.js smart contract and web app in VSCode for a Global Finance with blockchain use case](https://developer.ibm.com/patterns/global-financing-use-case-for-blockchain/)
## Tutorial 2: [Use IBM Blockchain Platform extension in VSCode to develop a Smart Contract](https://github.com/horeaporutiu/VSCodeTutorialBlockchain#use-ibm-blockchain-platform-extension-in-vscode-to-develop-a-smart-contract)  
## Tutorial 3: [How to quickly connect a Smart Contract to IBM Blockchain Platform Starter Plan using VSCode](https://github.com/horeaporutiu/VSCodeRemoteNetwork#vscoderemotenetwork) 
## Tutorial 4: [Run a commercial paper smart contract with the IBM Blockchain VSCode extension](https://developer.ibm.com/tutorials/run-commercial-paper-smart-contract-with-ibm-blockchain-vscode-extension/)
## [IBM Blockchain Platform in the IBM Cloud](https://console.bluemix.net/catalog/services/blockchain-platform-20)

<font size="+20">This is bigger text.</font>
A new VS Code extension provides smooth integration between smart contract development and network management, and you can now move from development, to test, to production in a single environment. The IBM Blockchain platform meets developers where they are, offering support for smart contracts to be written in JavaScript, Java, and Go languages.</font>
