# MarsKaseiCoinCrowdsale

## Description
This repository contains the Solidity smart contracts for the creation of KaseiCoin, a new cryptocurrency intended for use on the Mars colony, and its associated crowdsale system.

### Background:
Selected by the Martian Aerospace Agency, this project aims to develop a monetary system for Mars based on blockchain technology. KaseiCoin (Kasei meaning Mars in Japanese) is an ERC-20 compliant fungible token.

### Installation:
1. **Clone the repository:**
```bash
git clone https://github.com/regulolanz/MarsKaseiCoinCrowdsale.git
```

2. **Navigate to the repository directory:**
```bash
cd MarsKaseiCoinCrowdsale
```

3. **Install Dependencies:**
   - **Node.js and NPM**: Ensure you have [Node.js](https://nodejs.org/) installed. NPM will be included in the installation.
   - **Truffle Suite**: Install the Truffle development environment using NPM:
     ```bash
     npm install -g truffle
     ```
   - **Ganache**: Download and install [Ganache](https://www.trufflesuite.com/ganache) for a personal Ethereum blockchain.
   - **MetaMask**: Download and install the [MetaMask](https://metamask.io/) browser extension for accessing Ethereum enabled applications in your browser.

### Contracts:
- `KaseiCoin.sol`: This contract defines the KaseiCoin as an ERC-20 token.
- `KaseiCoinCrowdsale.sol`: This contract manages the crowdsale for KaseiCoin, allowing users to send ether and receive KaseiCoin tokens in return.

### Deployment:
Follow the instructions provided in the assignment to deploy the contracts onto a local blockchain using tools like Remix, MetaMask, and Ganache.

### Evaluation Evidence:

**For illustrative evidence of the project's implementation, please refer to the `Resources` folder.**

- **Screenshots**:
  - `Resources/Contract_Deployment.png`: A screenshot showcasing the successful deployment of the contracts.
  - `Resources/Token_Transaction.png`: A screenshot depicting a successful transaction of KaseiCoins.
  - `Resources/Crowdsale_Contribution.png`: An image showcasing a successful ether contribution to the crowdsale and the corresponding KaseiCoin allocation.
  
- **Videos**:
  - `Resources/Contract_Deployment_Demo.mp4`: A video demonstration of deploying the contracts onto the local blockchain.
  - `Resources/KaseiCoin_Transaction_Demo.mp4`: A video showing the process of transacting KaseiCoins between accounts.

### Optional Extensions:
To enhance the basic functionality of the crowdsale contract, we can integrate it with OpenZeppelin contracts like `CappedCrowdsale`, `TimedCrowdsale`, and `RefundablePostDeliveryCrowdsale`.

For detailed steps on how these extensions can be added, refer to the original assignment instructions or [OpenZeppelin documentation](https://docs.openzeppelin.com/contracts/2.x/crowdsales).