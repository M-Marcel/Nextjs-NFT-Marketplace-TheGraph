# NextJS NFT Marketplace with TheGraph

*This repo has been updated for Goerli over Rinkeby.*

## 1. Git clone the contracts repo

In it's own terminal / command line, run: 

```
git clone https://github.com/M-Marcel/Nextjs-NFT-Marketplace-TheGraph
cd Nextjs-NFT-Marketplace-TheGraph
yarn
```

## 2. Deploy to goerli 

After installing dependencies, deploy your contracts to goerli:

```
yarn hardhat deploy --network goerli
```

## 3. Deploy your subgraph

```
cd ..
git clone https://github.com/M-Marcel/nft-marketplace-thegraph
cd nft-marketplace-thegraph
yarn
```

Follow the instructions of the [README](https://github.com/M-Marcel/nft-marketplace-thegraph/blob/main/README.md) of that repo. 

Then, make a `.env` file and place your temporary query URL into it as `NEXT_PUBLIC_SUBGRAPH_URL`.


## 4. Start your UI

Make sure that:
- In your `networkMapping.json` you have an entry for `NftMarketplace` on the goerli network. 
- You have a `NEXT_PUBLIC_SUBGRAPH_URL` in your `.env` file. 

```
yarn dev
```
