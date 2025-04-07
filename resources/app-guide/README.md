---
description: A Comprehensive Guide to Using the Falcon App
---

# App Guide

### **How the Falcon App Works**

Falcon has two types of tokens :

* **USDf (Overcollateralized Synthetic Dollar):** A synthetic digital asset that is fully backed by eligible deposits, including stablecoins (e.g., USDT, USDC, FDUSD) and non-stablecoin assets such as BTC, ETH, stETH, and select altcoins. Stablecoin deposits mint USDf at a 1:1 ratio, while non-stablecoin assets are subject to an overcollateralization ratio to preserve protocol integrity.
* **sUSDf (Yield-Bearing Asset):** A yield-bearing token minted when USDf is deposited and staked into Falcon Finance’s ERC-4626 vaults. The value of sUSDf increases over time, as the protocol accrues yield through strategies such as positive & negative funding rate spreads, and altcoin staking. The sUSDf-to-USDf ratio reflects cumulative yield performance.

### **User Flow for Stablecoins Deposits**

**Step 1: Mint USDf**\
Begin by connecting a whitelisted Web3 wallet. Users may deposit eligible stablecoins (e.g., USDT, USDC, FDUSD) into their Falcon Account and mint USDf on a 1:1 basis relative to the deposited stablecoin value.

**Step 2: (Optional) Stake USDf to Receive sUSDf**\
Users can choose to stake their minted USDf into Falcon's vaults to receive sUSDF, a yield-bearing token that increases in value over time.

**Step 3: (Optional) Boost Yields via Fixed-Term Restaking of sUSDf**\
To earn boosted yield, users may also opt to restake sUSDf into fixed-term vaults (e.g., 3 or 6 months). Upon doing so, Falcon issues an ERC-721 NFT representing the locked-up assets, and accrues additional yield. Upon maturity, users can redeem their NFT for sUSDf.\
&#xNAN;_&#x41;lternatively, users may utilize the Express Mint feature to directly restake their deposits and mint an ERC-721 NFT at Step 1, bypassing Step 2 entirely._&#x20;

**Step 4: Unstake sUSDf to Receive USDf**\
While unstaking sUSDf, users will receive USDf at the prevailing sUSDf-to-USDf value.&#x20;

**Step 5: Redeem USDf for Stablecoins**\
Users may finally redeem USDf for their original stablecoin-denominated deposits (USDT, USDC, or FDUSD) on a 1:1 basis, subject to 7-days cooldown period.

### **User Flow for Non-Stablecoins Deposits**

**Step 1: Mint Overcollateralized USDf**\
Similarly, users begin by connecting a whitelisted Web3 wallet. They may then deposit supported non-stablecoin assets—such as ETH, BTC, stETH, or other accepted tokens.\
Upon deposit, the protocol applies an Overcollateralization Ratio (OCR) based on the asset’s risk profile and market volatility. This ensures that the USDf minted subsequently is backed by collateral of equal or greater value.

**Step 2: (Optional) Stake USDf to Receive sUSDf**\
Users can choose to stake their minted USDf into Falcon's vaults to receive sUSDF, a yield-bearing token that increases in value over time.

**Step 3: (Optional) Boost Yields via Fixed-Term Restaking of sUSDf**\
To earn boosted yield, users may also opt to restake sUSDf into fixed-term vaults (e.g., 3 or 6 months). Upon doing so, the protocol issues an ERC-721 NFT representing the locked-up assets, and accrues additional yield. Upon maturity, users can redeem their NFT for sUSDf.\
&#xNAN;_&#x41;lternatively, users may utilize the Express Mint feature to directly restake their deposits and mint an ERC-721 NFT at Step 1, bypassing Step 2 entirely._

**Step 4: Unstake sUSDf to Receive USDf**\
While unstaking sUSDf, users will receive USDf at the prevailing sUSDf-to-USDf value ratio. At the same time, users who initially deposited non-stablecoin assets will also receive an overcollateralization buffer. This is based on current market conditions:

* If the current market price is less than or equal to the initial mark price (of their deposit asset), the user may reclaim the full unit amount of the buffer.
* If the current market price is greater than the initial mark price, the user will reclaim a USD-equivalent value of the buffer based on the initial mark price.

**Step 5: Select Redemption Type** \
Once sUSDf has been converted into USDf and the overcollateralization buffer, users may select one of three options for final redemption:

* Full Redemption in Stablecoins
  * Convert their total claim—USDf value and overcollateralization buffer, into eligible stablecoins (e.g., USDT, USDC, FDUSD) at a 1:1 ratio. A 7-day cooldown period will apply.
* Split Redemption: Stablecoins + Original Collateral
  * Redeem part of their claim in stablecoins, and the remainder in the originally deposited non-stablecoin asset.
* Full Redemption in Original Collateral
  * Users may opt to redeem their total claim fully in the originally deposited collateral, subject to market pricing and availability.

_For an extensive description for terms used within the App Guide, users can refer to the_ [_Glossary_](../glossary.md) _section._

{% content-ref url="../glossary.md" %}
[glossary.md](../glossary.md)
{% endcontent-ref %}
