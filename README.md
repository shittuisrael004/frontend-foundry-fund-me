# Foundry Fund Me Front-End

*[⭐️ From (2:37:02) | Lesson 8: HTML Fund Me | By Patrick Collins](https://www.youtube.com/watch?v=sas02qSFZ74&t=9422s)*

This is a minimalistic example of what you can find in the [metamask docs](https://docs.metamask.io/guide/create-dapp.html#basic-action-part-1).

# Requirements

- [git](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git)
  - You'll know you've installed it right if you can run:
    - `git --version`
- [Metamask](https://metamask.io/)
  - This is a browser extension that lets you interact with the blockchain.
- [Live Server](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer) (Optional)
  - This is a VSCode extension that lets you launch a development local Server with live reload feature for static & dynamic pages

# Quickstart

1. Clone the repo

```
git clone https://github.com/Cyfrin/html-fund-me-f23
cd html-fund-me-fcc
```

2. Run the file.

You can usually just double click the file to "run it in the browser". Or you can right click the file in your VSCode and run "open with live server".

And you should see a small button that says "connect".

![Connect](connect.png)

Hit it, and you should see metamask pop up.

# Execute a transaction

If you want to execute a transaction follow this:

Make sure you have the following installed:

1. You'll need to open up a second terminal on VSCode and run:

```
git clone https://github.com/Cyfrin/foundry-fund-me-f23
cd foundry-fund-me-f23
make build
make anvil
```

Then, in a second terminal
```
make deploy
```

This will deploy a sample contract and start a local hardhat blockchain.

2. Update your `constants.js` with the new contract address.

In your `constants.js` file, update the variable `contractAddress` with the address of the deployed "FundMe" contract. You'll see it near the top of the hardhat output.

3. Connect your [metamask](https://metamask.io/) to your local hardhat blockchain.

> **PLEASE USE A METAMASK ACCOUNT THAT ISNT ASSOCIATED WITH ANY REAL MONEY.**
> I usually use a few different browser profiles to separate my metamasks easily.

In the output of the above `make anvil` command in the first terminal, take one of the private key accounts and [import it into your metamask.](https://metamask.zendesk.com/hc/en-us/articles/360015489331-How-to-import-an-Account)

Additionally, add your localhost network with **RPC URL:** *http://127.0.0.1:8545* and  **CHAINID:** *31337* to your metamask.

1. Refresh the front end, input an amount in the text box, and hit `fund` button after connecting

# Thank you!

If you appreciated this, feel free to follow [Patrick Collins](https://twitter.com/PatrickAlphaC) or donate!

ETH/Arbitrum/Optimism/Polygon/etc Address: 0x9680201d9c93d65a3603d2088d125e955c73BD65

[![Patrick Collins Twitter](https://img.shields.io/badge/Twitter-1DA1F2?style=for-the-badge&logo=twitter&logoColor=white)](https://twitter.com/PatrickAlphaC)
[![Patrick Collins YouTube](https://img.shields.io/badge/YouTube-FF0000?style=for-the-badge&logo=youtube&logoColor=white)](https://www.youtube.com/channel/UCn-3f8tw_E1jZvhuHatROwA)
[![Patrick Collins Linkedin](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/patrickalphac/)
[![Patrick Collins Medium](https://img.shields.io/badge/Medium-000000?style=for-the-badge&logo=medium&logoColor=white)](https://medium.com/@patrick.collins_58673/)
