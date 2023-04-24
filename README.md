# Sample Hardhat Project

This project demonstrates a basic Hardhat use case. It comes with a sample contract, a test for that contract, and a script that deploys that contract.

Try running some of the following tasks:

```shell
npx hardhat help
npx hardhat test
REPORT_GAS=true npx hardhat test
npx hardhat node
npx hardhat run scripts/deploy.js
```

This projects is designed to test Faucet.sol using Hardhat as well as the Chai testing library. 

In faucetsTests.js. Two tests are carried out:

1. To make sure that the owner of the contract is the person who initiated the Faucet contract. 
2. To make sure that no more than 0.1 ETH can be withdrawn at a time. 

There should also be a self destruct test. However, due to "pragma solidity 0.8.19;" in the Faucet.sol file
Any further updates means that the selfDestruct() function has been deprecated. Therefore, it can not be 
tested for. 
