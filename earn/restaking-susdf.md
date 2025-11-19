---
description: >-
  Read about restaking in Falcon Finance: fixed-term periods to earn enhanced
  yields represented by ERC-721 NFTs of locked positions.
---

# Restaking sUSDf

In exchange for boosted yield, Falcon allows users to restake their sUSDf holdings for a fixed-term tenure. This lock-up period can be selected by users from a range of available options, including a 3-month tenure, a 6-month tenure, and others, with longer periods providing higher yields. These fixed periods without redemption allows Falcon to optimize for time-sensitive yield strategies, generating higher yields for users. Upon restaking, the protocol mints and issues a unique ERC-721 non-fungible token (NFT) to users, representing their locked position.

### ERC-721

[ERC-721](https://ethereum.org/en/developers/docs/standards/tokens/erc-721/) is a standard non-fungible tokens (NFTs) on EVM-compatible blockchains. It provides a set of guidelines for creating unique digital assets that cannot be exchanged on a one-to-one basis due to their unique properties.

Falcon utilizes the ERC-721 NFT standard to record each user's unique restaked position, based on their staked sUSDf amount and selected fixed-term tenure. Viewable on Etherscan, each NFT will depict the details regarding users' unique locked positions.&#x20;

<figure><img src="../.gitbook/assets/Screenshot 2025-04-16 at 11.29.53 AM (1).png" alt="" width="563"><figcaption></figcaption></figure>

<table><thead><tr><th width="212">Term</th><th>Description</th></tr></thead><tbody><tr><td>Principal</td><td>Principal refers to the initial amount of sUSDf restaked by the user.</td></tr><tr><td>Rewards</td><td>Rewards refer to the amount of sUSDf accumulated as boosted yield.</td></tr><tr><td>Start Time</td><td>Start Time refers to the <a href="https://www.unixtimestamp.com/">Unix timestamp</a> of the user's time of restaking.</td></tr><tr><td>Duration</td><td>Duration refers to the total lock period selected by the user in seconds.</td></tr><tr><td>Maturity</td><td>Maturity refers to the <a href="https://www.unixtimestamp.com/">Unix timestamp</a> of the end of the lock period.</td></tr><tr><td>Status</td><td>Status reflects the current state of the user's locked position </td></tr></tbody></table>

At the end of their selected fixed-term tenures, users will be able to redeem their ERC-721 NFTs for their balance of sUSDf, which includes their initial restaked amount and any accrued boosted yield.

Refer to the [Boosted Yield](../resources/quick-app-guide/navigating-the-earn-tab/boosted-yield/) section for further details on the restaking process.

