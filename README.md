# 🚀 ERC20 Token Smart Contract with Hardhat 🎯
Welcome to the **Hardhat ERC20 Token** project! This repository contains a fully-functional ERC20 token smart contract built using Hardhat, deployed to the Ethereum testnet. Perfect for learning, experimenting, and integrating your very own custom token! 🌐

## Features 💡
- 🛠️ Hardhat for development: Compile, test, and deploy with ease.
- 💰 ERC20 Standard: Fully compliant token implementation.
- 🧪 Test suite: Comprehensive tests to ensure your token works flawlessly.
- 🌐 Deploy to testnets: Ready to launch on Rinkeby, Goerli, and more!
## Get Started ⚡
1. Clone the repo 🔗
2. Install dependencies 📦
3. Deploy and test your token on the blockchain 🚀
- **💼 Ideal for:** Smart contract developers, blockchain enthusiasts, and those building decentralized applications (DApps)!

# Getting Started

## Requirements

- [git](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git)
  - You'll know you did it right if you can run `git --version` and you see a response like `git version x.x.x`
- [Nodejs](https://nodejs.org/en/)
  - You'll know you've installed nodejs right if you can run:
    - `node --version` and get an ouput like `vx.x.x`
- [Yarn](https://classic.yarnpkg.com/lang/en/docs/install/) instead of `npm`
  - You'll know you've installed yarn right if you can run:
    - `yarn --version` And get an output like `x.x.x`
    - You might need to install it with npm

## Quickstart

```
git clone https://github.com/jopaleti/hardhat-erc20-token.git
cd hardhat-erc20-token
yarn
```

### Typescript (Optional)

```
git checkout typescript
```

# Usage

Deploy:

```
yarn hardhat deploy
```

# Deployment to a testnet or mainnet

1. Setup environment variabltes

You'll want to set your `SEPOLIA_RPC_URL` and `PRIVATE_KEY` as environment variables. You can add them to a `.env` file, similar to what you see in `.env.example`.

- `PRIVATE_KEY`: The private key of your account (like from [metamask](https://metamask.io/)). **NOTE:** FOR DEVELOPMENT, PLEASE USE A KEY THAT DOESN'T HAVE ANY REAL FUNDS ASSOCIATED WITH IT.
  - You can [learn how to export it here](https://metamask.zendesk.com/hc/en-us/articles/360015289632-How-to-Export-an-Account-Private-Key).
- `SEPOLIA_RPC_URL`: This is url of the sepolia testnet node you're working with. You can get setup with one for free from [Alchemy](https://alchemy.com/?a=673c802981)

2. Get testnet ETH

Head over to [faucets.chain.link](https://faucets.chain.link/) and get some tesnet ETH. You should see the ETH show up in your metamask.

3. Deploy

```
yarn hardhat deploy --network sepolia
```

## Verify on etherscan

If you deploy to a testnet or mainnet, you can verify it if you get an [API Key](https://etherscan.io/myapikey) from Etherscan and set it as an environemnt variable named `ETHERSCAN_API_KEY`. You can pop it into your `.env` file as seen in the `.env.example`.

In it's current state, if you have your api key set, it will auto verify sepolia contracts!

However, you can manual verify with:

```
yarn hardhat verify --constructor-args arguments DEPLOYED_CONTRACT_ADDRESS
```

# Thank you!

If you appreciated this, feel free to follow me!

[![Patrick Collins Twitter](https://img.shields.io/badge/Twitter-1DA1F2?style=for-the-badge&logo=twitter&logoColor=white)](https://x.com/OpaletiSegun)
[![Patrick Collins Linkedin](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/oluwatobijohnson4)
