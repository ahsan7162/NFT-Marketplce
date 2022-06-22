# BlockChain_Project

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
