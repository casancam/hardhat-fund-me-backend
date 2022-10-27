# Sample Hardhat Project

Functionality: Fund a smart contract with any amount of ETH and withdraw it all to the contract owner wallet address.

This project demonstrates a basic Hardhat use case. It comes with a sample contract, a test for that contract, and a script that deploys that contract.

It has 2 main smart contracts. FundMe.sol, which is the smart contract I used to fund/withdraw funds from the smart contract and PriceConverter.sol, which converts the price to USD. There is also a "mock" contract used for the tests.

You can compile running "npx hardhat compile" or "yarn hardat compile".

To deploy them run "npx hardhat deploy" or "yarn hardhat deploy". It would first deploy the mock contract on an internal chain and then it will deploy "FundMe.sol" on the selected network. E.g. "yarn hardhat deploy --network goerli"

To run tests try "npx hardhat test". There are unit and staging tests (unit are tests for the mock contract and staging for the main contract once it's gonna be deployed".

There are 2 scripts: "fund.js" and "withdraw.js". You can run this scripts on a local network. 
Create the local network with "yarn hardhat node". Run your scripts as "yarn hardhat run scripts/fund.js --network localohost"

Try to make the code more efficient taking a look at the gas Estimator.
