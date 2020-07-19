# Overview of Unioracle 🔮

[Unioracle](https://unioracle.org) is a decentralized oracle protocol built on Uniswap.

Note that, this is NOT an official project from Uniswap. Unioracle is a project aimed to help the Uniswap ecosystem. Uniswap works in a fully trustless and decentralized way. We build Unioracle so that to enable a trustless and decentralized oracle system that is fully built on Uniswap.

As Uniswap grows rapidly, building DEFI products on top of Uniswap is possible, such as lending, futures, and options. Oracle is critical in DEFI to provide reliable and trustable price feeds.

However, building an oracle is quite challenging. As the Uniswap team puts: `Reliable oracle maintenance is a difficult task, and can become a point of failure in times of congestion. Instead, consider building this functionality directly into the critical calls of your own smart contracts, or incentivize oracle maintenance calls by other parties`.

Unioracle protocol is a decentralized oracle network incentivized by Uni Oracle (UNO) token. Whoever contributes to updating price information will receive UNO token.

# How it works 🔮
For the very first version, we want to keep it simple and minimal. We have deployed a Uniswap Interface with Unioracle supported on [Unioracle.org](https://unioracle.org). You could also build [Uniswap-Interface with Unioracle](https://github.com/Unioracle/uniswap-interface) locally to join Unioracle. While you are using Uniswap, the targeted trading pair price feed will get updated based on a fixed sliding window. For more information, please refer to [Uniswap Doc](https://uniswap.org/docs/v2/smart-contract-integration/building-an-oracle/). Unioracle reuse `ExampleSlidingWindowOracle` provided by Uniswap with minimal change. Check out on [Github](https://github.com/Unioracle/uniswap-v2-periphery/blob/master/contracts/examples/ExampleSlidingWindowOracle.sol) for more details.

Unioracle computes a 1-hour averaged price for each price feed oracle. Each oracle can be updated every 10 minutes. If your action happens to trigger an update on Unioracle, you will receive 10 UNO token. Meanwhile. Meanwhile, the Unioracle team will receive 10 UNO token.

# Open Source and Smart Contract
Unioracle Source code can be found on [Github](https://github.com/Unioracle). We have deployed the smart contracts on the Ethereum mainnet, and the Ropsten, Rinkeby, Görli, and Kovan testnets.

# Unioracle Token Info 🔮
Unioracle Token (UNO) [`0x523Bc523FdaDFF610e11fD78192CDb6a853de1F0`](https://etherscan.io/token/0x523Bc523FdaDFF610e11fD78192CDb6a853de1F0)

# Unioracle Oracle Contract 🔮
ExampleSlidingWindowOracle [`0x97376FDD337C743eDf3D5708599CB2dffeBcF609`](https://etherscan.io/address/0x97376FDD337C743eDf3D5708599CB2dffeBcF609)

# Unioracle Router Contract 🔮
UnioracleV2Router01 [`0xAA30167B16B41E3E85f126E8a9f41A3feBba0048`](https://etherscan.io/address/0xAA30167B16B41E3E85f126E8a9f41A3feBba0048)


# FAQ 🔮
**Q:** Is this a fork of Uniswap?

**A:** No. Unioracle fully relies on the Uniswap core framework. Users help to contribute Unioracle while using our slightly modified Uniswap Interface. All swaps and liquidity changes still happen on Uniswap.

**Q:** What is token economics of Uniorale Token (UNO)?

**A:** The complete token economics is not finalized yet. Since Unioracle is incentivized by UNO token, mining UNO token will be more and more difficult as time goes. To keep it clear and clean, each successful oracle update will generate 10 UNO token to the user, and 10 UNO token to the Unioracle team at the moment. As more users join, it will be harder to mine UNO token. Again, this is meant to be a community-driven project. We welcome Uniswap users to provide valuable technical supports and feedbacks. We will keep improving the token economics together with community growth.

**Q:** Will I receive UNO token when swapping on any trading pair?

**A:** Yes. Currently, we keep our oracle system permissionless and allow any user to provide price information on any trading pair. The goal is to allow UNO token being distributed widely among the Uniswap community. This might change as Unioracle token economics is under active development.

**Q:** Can I use Unioracle's oracle price feed in my project now?

**A:** Not yet. Unioracle just gets started. The reliability of the oracle will depend on how many users are collaboratively maintaining Unioracle. Only use the price feed when Unioracle is widely recognized. Also, popular trading pairs get updated more frequently, thus more reliable. Please carefully evaluate it when using Unioracle at this stage. More docs and tools are coming for developers.

**Q:** What is the token supply of UNO?
**A:** To make Unioracle widely adopted, we don't have a fixed token supply currently. However, there is an issuance rate for UNO token per trading pair, which is 20 UNO per 10 minutes. We will actively monitor the network growth and make sure UNO token brings positive incentives to Unioracle protocol.

# Sites
- [Unioracle](https://unioracle.org)

# Channels
- [Discord](https://discord.gg/bhWPVVX)
- [Github](https://github.com/Unioracle)
