# EthereumToPolygonNFTShift

This undertaking encompasses a basic ERC-721A smart contract designed to generate and oversee non-fungible tokens (NFTs). The contract enables users to produce fresh NFTs, define their metadata (URI), and verify NFT balances. Additionally, it provides the capability to transfer your NFTs to an alternate network through the FxPortal bridge, here Polygon .

## Note 
1. Make sure to add a .env file and add your account's Private Key in the file.
2. You can customize the number of NFTs to be minted and the base URL for the images in the batchMint.js script and the NFT.sol contract, respectively.
 
## Getting Started

1. Clone the repository:

2. Install the dependencies :

```
npm i
```

3. Install the ERC721A contract:

```
npm install erc721a
```

4. Compile the contract and deploy
```
npx hardhat run scripts/deploy.js --network goerli

```
To batch mint tokens: npx hardhat run scripts/BatchMint.js --network goerli

To approve and deposit your tokens to polygon: npx hardhat run scripts/BatchTransfer.js --network goerli


## Description
A 5-item NFT collection has been created using "Dalle". The items are stored on IPFS using pinata.cloud.  ERC721A smart contract is deployed to the Goerli Ethereum Testnet. There is a promptDescription function on the contract that returns the prompt used to generate the images.



## Technologies Used 
- MetaMask - Wallet and gateway to Ethereum blockchain  
- ethers.js - Library for interacting with Ethereum smart contracts  
- Hardhat - Development environment and task runner for building, testing, and deploying smart contracts on Ethereum and other blockchain platforms
## Authors
- [Utsav Koul](https://github.com/utsavkoul69)
