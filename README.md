# NFT Marketplace

## Introduction
In this project we created a NFT marketplace based on ethereum tokens. The basic purpose of this project was to create a portal for buying and selling of NFTs and make use of smart contracts developed using solidity.

## Technologies Used
- Solidity development environment : HardHat
HardHat provides us with a local environment for developing, deploying and debugging the smart contract using local machine. HardHat is local Ethereum network designed for development.
- Web3 API : Infura Network
It is a suite of high availability APIs and Developer Tools provide quick, reliable access to the Ethereum and IPFS networks
- Web application framework : Next.js
Next.js is fullstack framework based on the react.js to create UI and backend logic for web applications.
- Ethereum Web Client Library : Ethers.js 
The ethers.js library aims to be a complete and compact library for interacting with the Ethereum Blockchain and its ecosystem
- Wallet Software: Metamask
Available as a browser extension and as a mobile app, MetaMask equips you with a key vault, secure login, token wallet, and token exchange—everything you need to manage your digital assets.

## Architecture
![Blockchain Project drawio](https://user-images.githubusercontent.com/60193296/175040937-58108e15-75ab-4e9d-ba80-9e8177218184.png)

## Project Pre-requesite
1. Metamask Chrome Extension


## Clone the Project

```bash
git clone https://github.com/owaisimran2411/BlockChain_Project.git
```

## Project Initial Setup

After cloning the project, go to the directory where the project was download and execute the following commands
```bash
cd nft-marketplace
npm install
```

## Project Server Execution

Open three terminals into the same directory:
1. Terminal 1: Execute a Hardhat Node
```bash
npx hardhat node
```
2. Terminal 2: Deploy the nft and nft-marketplace contracts
```bash
npx hardhat run scripts/deploy.js --network localhost
```
After the contract is deployed on localhost, copy the nft market address and nft address and replace them in the file: ./config.js
```config.js
export const nftaddress = "***"             //replace '***' with copied nft-address
export const nftmarketaddress = "***"       //replace '***' with copied nft-market-address
```

3. Terminal 3: Execute the next.js server for web application
```bash
npm run next dev
```
After Terminal 3 is up and running goto the [website](http://localhost:3000)

## Project Execution

1. From terminal 1, copy private key for any of the 20 accounts provided and import that wallet into the metamask wallet. <br/>
**NOTE: YOUR METAMASK WALLET SHOULD BE RUNNING ON LOCALHOST**
2. In the web application, go to sell NFT option and list your NFT, you will see that your NFT is currently available for sale.



## Contributors
<b> The Project is Contributed by: </b>
* [Muhammad Owais (18K-0346)](https://github.com/owaisimran2411)
* [Muhammad Ahsan (18K-0260)](https://github.com/ahsan7162)
* [Syed Muhammad Owais (18K-0181)](https://github.com/SyedMuhammadOwais18)
