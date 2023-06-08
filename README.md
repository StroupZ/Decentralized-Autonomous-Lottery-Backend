# Decentralized Autonomous Lottery Backend
Link to frontend: https://github.com/StroupZ/Decentralized-Autonomous-Lottery
<br><br>
This is the backend/smart contract portion for the Decentralized Autonomous Lottery... a dApp which once deployed, initiates and concludes lotteries in succession over a predetermined period of time. The smart contract was written in solidity and deployed to the Goerli Testnet, enabling it to be decentralized, transparent, and immutable. It is complimented with thorough unit and staging tests.
<br><br>
## Tech Stack
- JavaScript for writing tests and scripts
- Solidity for writing smart contracts
- Ethers.js for testing and deploying smart contracts
- Hardhat for testing and deploying smart contracts
- Chainlink Automation for maintenance
- Chainlink VRF for verifiable randomness
<br><br>
## Use
1. Make sure you have an IDE and Node.js installed.
2. Clone this repo.
3. Run `yarn add` to install all dependencies.
4. Create a `.env` file with the following information:
   - `GOERLI_RPC_URL=YOUR_GOERLI_RPC_URL`
   - `PRIVATE_KEY=YOUR_PRIVATE_KEY`
   - `COINMARKETCAP_API_KEY=YOUR_COINMARKETCAP_API_KEY`
   - `ETHERSCAN_API_KEY=YOUR_ETHERSCAN_API_KEY`
   - `UPDATE_FRONT_END=true`
5. Run `yarn hardhat node` to deploy contracts on localhost.
6. Run `yarn hardhat deploy --network goerli` to deploy contracts on Goerli Testnet.
<br><br>
## Test
- Run `yarn hardhat test` to run unit tests on localhost.
- Run `yarn hardhat test --network goerli` to run staging tests on Goerli Testnet. Make sure to first register the lottery contract address with [Chainlink VRF](https://vrf.chain.link/goerli) and [Chainlink Automation.](https://automation.chain.link/goerli)
<br><br>
## Faucets
- [Goerli ETH](https://goerlifaucet.com/)
- [Goerli LINK](https://faucets.chain.link/goerli)
