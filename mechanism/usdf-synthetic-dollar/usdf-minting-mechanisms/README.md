---
description: >-
  A quick guide into minting mechanisms in Falcon Finance: getting USDf tokens
  with Classic Mint vs. Innovative Mint.
---

# USDf Minting Mechanisms

Falcon offers multiple pathways for users to mint USDf, providing flexibility based on individual asset holdings and strategic preferences.

Users can choose between two minting options: the [Classic Mint ](classic-mint.md)and the [Innovative Mint](innovative-mint.md).

Through the Classic Mint, users can mint USDf by depositing supported stablecoins such as USDT and USDC, or by using non-stablecoin assets such as ETH, BTC, or select altcoins. When minting with stablecoins, users receive USDf at a 1:1 ratio (subjected to prevailing market rates). For non-stablecoin deposits, an overcollateralization ratio is applied to ensure that the value of the collateral remains higher than the value of the USDf minted. The implementation of an OCR helps to mitigate the impact of market slippage and inefficiencies, ensuring that each USDf minted by all non-stablecoin deposits is fully backed by collateral of equal or greater value.

The Innovative Mint offers an alternative method for users seeking to mint USDf with non-stablecoin assets. Under this mechanism, users commit their collateral for a fixed term, enabling access to liquidity while maintaining defined participation in potential price appreciation. The amount of USDf minted is conservatively determined relative to the value of the collateral, based on parameters such as tenure, strike price multipliers, and capital efficiency levels, ensuring continuous overcollateralization. Collateral deposited to mint USDf is managed through neutral market strategies that minimize sensitivity to market movements, while preserving full asset backing. In periods of significant market volatility, the protocol implements appropriate liquidation procedures to ensure the integrity of the collateral backing.

Maintaining overcollateralization is fundamental to Falcon’s design. It ensures that every USDf minted is backed by collateral exceeding one dollar in value, reinforcing the security and stability of the synthetic dollar system.

