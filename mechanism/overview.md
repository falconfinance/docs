# Overview

The diagram below provides an overview of how users' deposits into Falcon are stored and utilized.&#x20;

<figure><img src="../.gitbook/assets/Screenshot 2025-04-17 at 7.33.03 PM.png" alt=""><figcaption></figcaption></figure>

There are several key parties that users should be aware of:

<table><thead><tr><th width="212">Party</th><th>Description</th></tr></thead><tbody><tr><td>Users</td><td>This refers to anyone who utilizes Falcon's range of features, such as depositing/withdrawing, minting/redeeming, staking/unstaking, and restaking/claiming.</td></tr><tr><td>Custodians / <br>OES Providers</td><td>This refers to third-party custodial solutions that Falcon employs to store and secure users' deposits. These include Ceffu (MirrorX), and Fireblocks (CVA).</td></tr><tr><td>Centralized Exchanges (CEXs)</td><td>These refer to the various centralized exchanges that Falcon employs yield generating strategies like price arbitrage on. These include Binance, and Bybit.</td></tr><tr><td>Liquidity Pools</td><td>These refer to the various venues that Falcon utilizes users' collateral to provide liquidity in exchange for yield.</td></tr><tr><td>Staking Pools</td><td>These refer to the various venues that Falcon stakes users' collateral to secure various networks in exchange for yield.</td></tr></tbody></table>

### General Flow of User Deposits

1. Users deposit collateral assets into Falcon - these can range from stablecoins to non-stablecoin assets. USDf is minted in return.
2. All user deposits are routed to third-party custodians where multi-signature (multi-sig) or multi-party computation (MPC) processes are in place to ensure that assets are stored in a secure manner.
   1. These processes require multiple approvals from separate, authorized signers before any withdrawal can occur. Consequently, there is no single individual or entity that can unilaterally remove or re-route assets.
   2. Falcon does not directly control or hold user-deposited assets in a way that would allow a single party to misappropriate them.
3. Falcon utilizes off-exchange settlement mechanisms that allow for "mirroring" of assets within the custodian accounts onto CEXs, where various strategies are deployed and trades are placed.
4. Falcon deploys a portion of assets into tier-1 on-chain liquidity pools to generate yield through on-chain dex activity and arbitrage.
5. Falcon stakes certain assets on-chain for chains with native staking capabilities to generate additional yield on spot holdings.
