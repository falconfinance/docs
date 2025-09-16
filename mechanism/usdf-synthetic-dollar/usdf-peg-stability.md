---
description: >-
  The explanation of how USDf synthetic dollar’s peg is kept using delta-neutral
  hedging, overcollateralization, and cross-market arbitrage.
---

# USDf Peg Stability

Falcon Finance maintains USDf’s peg stability through a combination of delta-neutral and market-neutral strategies. Collateral assets deposited to mint USDf are actively managed to neutralize directional exposure, minimizing the effects of individual asset price movements and broader market fluctuations. This ensures that fluctuations in the underlying collateral do not affect the value backing USDf.

In parallel, the protocol enforces strict overcollateralization requirements. By requiring that the value of deposited assets consistently exceeds the value of USDf minted, Falcon establishes a resilient buffer against volatility in non-stablecoin assets. This ensures that every USDf remains fully backed by assets of equal or greater value, reinforcing the strength of the peg stability.

Together, these mechanisms allow Falcon to maintain synthetic dollar stability, even during periods of significant market fluctuations.

### Cross-market Arbitrage

Falcon also utilizes arbitrage of USDf across both centralized and decentralized spot markets to maintain the peg of USDf. This opportunity is also available to users, who are able to mint or redeem to profit from the price differences of USDf.

* If USDf is above peg (> $1.00):
  * KYC-ed Users can mint USDf at peg via Falcon, and sell them on external markets where USDf is trading above peg value.
* If USDf is below peg (< $1.00):
  * KYC-ed Users can purchase USDf below peg on external markets and redeem them for $1.00 worth of collateral per token via Falcon.

This incentivizes all parties to actively take part in stablizing USDf at its rightful peg value across various markets.
