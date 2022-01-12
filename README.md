# Deploy an NFT project on Ethereum

## myFirstNFT

Create and deploy the NFT on the Ethereum devnet by following this [tutorial](https://ethereum.org/en/developers/tutorials/how-to-write-and-deploy-an-nft/)

to run the project: 
- you need to have a Metamask wallet, a address to send and receive transactions, and switch to Ropsten test network to deploy our smart contract to the test network.

- secondly Alchemy account, a blockchain developer platform and API that allows us to make requests to the Ethereum blockchain, and create your app. 

don't forget to set those environement variables to connect METAMASK & ALCHEMY to your project:

API_URL: HTTP Alchemy API URL

PRIVATE_KEY: your private key from MetaMask

PUBLIC_KEY: your public account address

Steps followed:
-Start Hardhat Project : Hardhat is a development environment to compile, deploy, test, and debug your Ethereum software.

-Write NFT Smart Contract Code.

-Compile the contract : npx hardhat compile

-Deploy the contract : npx hardhat --network ropsten run scripts/deploy.js (you'll get the deployment adress, and check in the Ropsten etherscan that it has been deployed successfully)
  
-store the NFT asset and metadata in Pinata, a convenient IPFS API and toolkit, to store our NFT asset and metadata.

-Mint token : node scripts/mint-nft.js

-add the collectable to METAMASK

Using the mint-nft.js you can mint as many NFT's as your heart desires! Just be sure to pass in a new tokenURI describing the NFT's 
metadata (otherwise, you'll just end up making a bunch of identical ones with different IDs).
