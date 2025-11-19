---
description: >-
  Description of the Classic Mint process in Falcon Finance for minting USDf
  with stablecoin or non-stablecoin collateral.
---

# Classic Mint

_**Disclaimer: The minimum amount required to initiate an Classic Mint is USD$10,000 worth of eligible stablecoin and non-stablecoin collateral. Users should contact support@falcon.finance for more information or assistance with the process.**_

<figure><img src="../../../.gitbook/assets/Flowchart V10 - Whitepaper.png" alt="" width="563"><figcaption></figcaption></figure>

**Stablecoins vs Non-Stablecoin Assets**\
Users minting USDf with stablecoins will do so at a 1:1 ratio, while users minting with non-stablecoin assets will be subject to an overcollateralization ratio (OCR). As indicated in the previous section, OCRs will vary based on the non-stablecoin asset's risk profile.

Refer to the [App Guide](../../../resources/quick-app-guide/) for further details on different deposit processes.

**Express Mint**\
An Express Mint is an extra feature provided for users using the Classic Mint mechanism. It offers users two additional options in the process of minting their USDf. Compared to a regular mint where users simply receive the amount of USDf minted, and are required to proceed with further processes like staking and restaking manually, Express Mint users are able to bypass these automatically.

* Option 1: Mint & Stake
  * This option automatically stakes users' USDf after it is minted, directly returning users sUSDf instead of USDf at the end of the process.
* Option 2: Mint, Stake, & Restake
  * This option requires users to pick between available fixed-term tenures, automatically staking their' USDf after it is minted, then restaking the returned sUSDf into the chosen vaults.
  * Users will receive an ERC-721 NFT representing their locked position instead of USDf or sUSDf at the end of the process

Refer to the [sUSDf](../../../earn/susdf-yield-bearing-token.md) and [Restaking](../../../earn/restaking-susdf.md) sections for further details on staking and restaking respectively.
