---
layout: post
title: The Big Update and Web3 Pass
author: joshua
---

# The Big Update and Web3 Pass

Of the past several weeks, we have made some incredible progress, and are really exited to share with all of you. Each one is a major add-on to the existing RSS3 protocol, and will further help us build toward the world of Web3.

## The Big Update

Starting from the beginning of the Internet, human beings have been creating assets online. Assets are not only about finance: all that you create or own in the cyber world are your assets. These started with simple contents on a self-hosted website, then went to more sophisticated datasets through different applications. Nowadays, with the advancement of decentralized infrastructures, we are seeing much more assets online like tokens and NFTs. We definitely are not going to stop there. If we take a look at the trend, it is easy to tell that the quantity and variety of online assets have been increasing for all the time being. Specifically, we expected to see more non-transferrable tokens and gaming assets in the next few years.

The next era belongs to the Metaverse, within which users will be creating more and heavier online assets through different applications, most likely on decentralized networks. The truth is that we cannot expect all assets to be on the same network. Or if they were on the same network, we cannot expect them to be of the same standards. Even for now, we see users with tokens on different chains with a majority on Ethereum, gaming NFTs like Axie Infinity on chains like Ronin, and articles and videos stored in a decentralized way on Arweave and IPFS. This is not determined by the users who always expect things to be simple, but by the underlying logic of these technologies that cannot be solved in a short time. Also, it might be better this way since it limits the harm of a possible, only in theory probably, single decentralized network failure (SDNF).

Assets' Interoperability across different applications will be achieved with much less effort this way. Right now, the way applications handle interoperability is by looking onto each chain, and searching for and verify the assets. If Metaverse applications are to handle as many cross-network assets as possible for better user experience and engagement, they will need a better way searching and verifying these assets. RSS3 files will be the trustless way for that, though we are still on our way of decentralization. To make things even easier, we will be introducing Web3 Pass as the simplest, the most adaptive, and the most powerful way for applications to use as trustless user profiles.

That major update restates the fundamental position of RSS3.

### As a Cross-Network Aggregator

RSS3 is destined to become the indexer for any cyber persona, and we are adding verification and indexing modules to the protocol. RSS3Hub (or later the RSS3 nodes) will be able to verify ownership of given specific account, and then index the assets from verified accounts into the RSS3 files. And network does not only refer to decentralized networks, but also existing centralized platforms as well. Specifically, we are adding RSS3Account and RSS3Asset into the RSS3 Standard, and RSS3Hub will be first experimenting these new modules together with the introduction of the Web3 Pass™. We will soon release more information regarding the update and how community developers can easily implement these modules as well.

### As a User-Controlled Index

It goes without saying that RSS3 does not stop with simply being an aggregator. If we look at the ways how users or addresses are showing their assets now, they are using the most primitive way. If you have 700 NFTs, then they will be displayed at once and the only options for the viewers are most likely to be pricing or chronology orders. The human touch is missing. And that's where RSS3 files come into play. With the enhanced RSS3Hub (which will later turn into RSS3 nodes), assets across different networks will be gathered, and for the first time in Web3 history, users are granted with the power to control this index. They can choose to show or hide any asset, and they are free to modify the order themselves. All your fans and friends will see your best collections, contents or achievements from your own index, in your own way. 

![Untitled](https://i.imgur.com/pqoVFBC.png)

## OneSign™

When we first shipped out the RSS3 protocol, we designed it in a data-ownership first way, which requires a separate signature every time when the user makes a change. This is the simplest way for security, but definitely not good enough for social and content applications: they don't need to be confirmed for every action. So in this big update, we are introducing the new signing architecture called OneSign, which will completely change identity verification for non-financial dApps, making it more secure and convenient. And no, we haven't patented it lol and we want to call for all non-financial dApps, whether already adopting a similar architecture or not, to form an open standard called OneSign.

First of all, the private key for signing non-financial apps and financial apps should be different, eliminating possible security risks. At the same time, users should gradually form a conceptual model where different types of keys will be used for different cases.

- Specifically, if it is for financial purposes:
    1. Always make sure that SIGN IT IF YOU MEAN IT, which means that users' actions have to be explicitly signed before execution.
    2. Private keys should never leave wallet apps.
- However, if it is for non-financial purposes:
    1. Users don't need to explicitly sign for most actions (this is not only to meet the already-formed user cognition in the web2 era, it also just makes sense since most actions do not carry that much stake. E.g. even secure messaging apps won't explicitly ask for signature every time when messages are signed).
    2. Private keys can be stored in secure local storages like IndexedDB, also making sure that no application or extension can access these keys.

In order for RSS3 to still work with Ethereum, it makes sense to still use the Secp256k1 curve. However, as stated before, we need to avoid letting users sign social or content actions directly with the Ethereum key. So we will generate another key pair for the users, use the Ethereum private key to sign the generated public key, and finally store the newly generated private key into IndexedDB. This way, users will need to sign with their Ethereum private keys only when they are generating the new key pair. Of course, as an advanced option, users are allowed to force to regenerate a key pair every time they sign an RSS3 action, or they can also set an expiration time.

We can't predict what the resourceful black-hat hackers would do, but what we can do is to make sure that we use a different curve for the generated key pair, making it valueless. 

We call for the Web3 industry to make this a universal standard: whenever a user is signing with an Secp256k1 private key, it is a sensitive operation, and if not so, then the operation won't carry much stake. We don't want users to keep checking the actions they sign when it's only for following their friends. The standard of signing contents have long existed, mostly with Curve25519. It was actually the emergence of Bitcoin that gradually made Secp256k1 an industry standard. Thus, it makes sense for us to keep separated curves for different purposes.

There are lots of great choices for a curve different from Secp256k1. For OneSign, we choose Curve25519, one of the most widely tested and used choices. And we welcome any discussion with the choices we made here.

We are clear that RSS3 is not the first project that is trying to adopt a signing architecture like this. Lots of social media, messaging and other decentralized applications have trailblazed on this direction. But we hope an open and shared standard can be made, and we hope all who work on non-financial decentralized apps can join us.

## Web3 Pass™

Here comes our "One More Thing..."

For the past several weeks, we have been secretly developing something that can show you the power of RSS3 right at your fingertips. And it's called the Web3 Pass.

With the advanced RSS3 protocol, we believe it's time to come up with a native way for users to interact with their RSS3 files and show off their cyber assets. We will be gradually shipping more and more modules onto the Web3 Pass and showing more of what RSS3 can do. Developers will not only benefit from this open Web3 User Table, but also these beautify user profile pages that are ready to be shown right in your applications, and they fit every device and platform. And all these will take just one line of code.

You can start your RSS3-based Web3 Pass easily with your existing Ethereum address, and start your cross-network metaverse Web3 journey. It will be extremely secure and easy thanks to the OneSign architecture mentioned above. 

We will be experimenting first through the Ropsten Network with a simple guide here: [https://www.notion.so/rss3/A-Brief-Guide-for-Web3-Pass-3f42b829d0d64815aca63602cbe4ebaf](https://www.notion.so/A-Brief-Guide-for-Web3-Pass-3f42b829d0d64815aca63602cbe4ebaf).

Note that all data will be transferred to mainnet once we are ready to move.

### RSS3 Naming Service

The first thing is about the RSS3 Naming Service. It's still not well developed, but we believe it's time for us to run a trial with the Web3 Pass. Every user needs to register through the Ethereum contract ([https://ropsten.etherscan.io/address/0x63cfeb343975116ec2fc27125609da236d066615#code](https://www.notion.so/3975116ec2fc27125609da236d066615)) to get started. This registration will cost you to burn a $PASS token ([https://ropsten.etherscan.io/address/0x63cfeb343975116ec2fc27125609da236d066615#code](https://www.notion.so/3975116ec2fc27125609da236d066615)), and grants you an RNS which is a type of ENS. This may resemble with Mirror.xyz's registration, but as a special type of ENS, one address can only have one RNS, it won't be transferable, and it will never expire. Also, you can register a regular ENS for another address, but not for RNS.

We designed RNS to be this way so that it will not be considered as a typical asset. As a unified resolver for a decentralized cyber persona, it just does not make sense for anyone to carry two, or give or trade it to another persona. Consider how someone won't have multiple or trade passports, or at least in most cases. For now, any RNS has to be at least 2 characters with maximum of 15. And we did leave a future option for changing one's RNS, but that's not for us to decide, but the RSS3 DAO on how this should work.

### Verify and control

As discussed in the big update, RSS3 protocol now allows you to verify the ownership of a given account. For this first version, we are going to support the verification of Ethereum and Binance Smart Chain. Their verifications are very straightforward: Through your Web3 Pass, just click on adding a new account, choose which network this account is based upon, and then sign a message with your MetaMask extension. Note that right now, adding and verifying account can only be done with MetaMask or similar browser extension. And we are working on making WalletConnect work so this can be done through a mobile device as well. At the same time, you can always log into your Web3 Pass with WalletConnect, manage your Pass and check on others Pass. We will be working hard on getting more accounts support onboard, including different chains, side chains, decentralized networks and even centralized platform. But for now, you can try and go enjoy showing all your collections from however many ETH and BSC wallets you want, as long as they belong to you 😉

Once your accounts have been verifies, assets will be pulled into your RSS3 file shown to you through your Web3 Pass. Now, you can drag and drop all these collections anyway you want. You can choose to hide most of them but only show a few of your best, or you can go ahead and click on display all, in which case all will be show on your Pass.

This way, your verified and aggregated Pass with your own touch is initiated. Take your link and hang it somewhere conspicuous like your Twitter so that others can follow your Pass and look it up from time to time. 

## Some QAs

- Who developed the Web3 Pass?

    It's developed by us, Natural Selection Labs, the same people behind RSS3.

- What is RNS?

    It's a special type of ENS developed by us, granted to any address when registering for the Web3 Pass

- What is $PASS?

    It's an ERC-20 Token we released. Every time an address is trying to register for the Web3 Pass, 1 $PASS is required to be burnt. 

- How do I get $PASS?

    $PASS is **NOT** sold anywhere through any exchange, centralized or decentralized. The only way of getting a $PASS for now is to join the waitlist here ([https://form.typeform.com/to/ds3gKvwB](https://form.typeform.com/to/ds3gKvwB)).

- Why do this burn thing?

    For the early stage, it's a way of limiting the number of users. For a later stage, it might turn into a more radical-market way for the right to register.

- Why choose ETH and BSC?

    They are popular and easy to implement.

- What is the relationship between RSS3 and Web3 Pass?

    They are projects led by the same company. Web3 Pass is based on the RSS3 Protocol.

- Can I build something similar to the Web3 Pass?

    Yes, the RSS3 Protocol and all index files are open. We actually hope that you develop something much better than the Web3 Pass.

- Are you making money from the registration of Web3 Pass?

    No, you can check on EtherScan ([https://ropsten.etherscan.io/address/0x63cfeb343975116ec2fc27125609da236d066615#code](https://www.notion.so/3975116ec2fc27125609da236d066615)) regarding or smart contract. All the ETH you pay is to miners of the Ethereum network. We actually will be paying FOR YOU when migrating to mainnet later on.

- Will you airdrop any token for early Web3 Pass users?

    That sounds reasonable but it's still under discussion.

- Who led this big update on RSS3 Protocol?

    DIYgod and Atlas from Natural Selection Labs.

- Who exactly is behind Web3 Pass?

    Anny, Atlas, Candinya, DIYgod and Johnny.

- Who is making sure that I will know about these updates?

    Usagi and Seiyo.

- Who is taking care of the team?

    STZ.

- Who came up with all these names (Web3 Pass, OneSign, RNS)?

    The Chief Naming Officer, Joshua.
