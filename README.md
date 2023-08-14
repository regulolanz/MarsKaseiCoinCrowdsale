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
   - **Ganache**: Download and install [Ganache](https://www.trufflesuite.com/ganache) for a personal Ethereum blockchain.
   - **MetaMask**: Download and install the [MetaMask](https://metamask.io/) browser extension for accessing Ethereum enabled applications in your browser.

### Contracts:
- `KaseiCoin.sol`: This contract defines the KaseiCoin as an ERC-20 token.
- `KaseiCoinCrowdsale.sol`: This contract manages the crowdsale for KaseiCoin, allowing users to send ether and receive KaseiCoin tokens in return.

### Deployment:
1. **Setting up your Local Blockchain with Ganache:**
    - Launch Ganache.
    - You should see 10 test accounts with 100 ETH in each.
    - Take note of the mnemonic phrase provided. This will be used to connect MetaMask to your local blockchain.

2. **Configuring MetaMask:**
    - Open MetaMask in your browser.
    - Click on the network dropdown (typically shows "Main Ethereum Network").
    - Select "Custom RPC" and enter the details of your Ganache instance (usually `HTTP://127.0.0.1:7545`).
    - Import an account using the private key from one of your Ganache's test Ethereum accounts.

3. **Deploying with Remix:**
    - Open [Remix](https://remix.ethereum.org/) in your browser.
    - Import the `KaseiCoin.sol` and `KaseiCoinCrowdsale.sol` contracts.
    - Compile both contracts.
    - Change the environment in the Remix `Deploy & Run Transactions` tab to `Injected Web3`. This allows Remix to connect to your MetaMask.
    - Deploy the `KaseiCoin.sol` contract first.
    - After successfully deploying the KaseiCoin contract, deploy the `KaseiCoinCrowdsale.sol` contract. 

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