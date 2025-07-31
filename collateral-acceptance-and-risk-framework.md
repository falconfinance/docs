# Collateral Acceptance & Risk Framework

Falcon Finance maintains a data‑driven framework for selecting the **Supported Collaterals** that can be pledged to mint USDf. The objective is to safeguard USDf’s peg and ensure that all accepted assets exhibit sufficient market liquidity, price transparency, and risk‑adjusted resilience.

> These guidelines are reviewed periodically and may be updated in response to evolving market conditions or regulatory requirements.

### Eligibility Screening Workflow

<table><thead><tr><th width="40"></th><th width="141.91015625">Stage</th><th>Check </th><th width="395.6328125">Decision Logic</th></tr></thead><tbody><tr><td>1</td><td>Primary Listing </td><td>Is the token listed on Binance Markets?</td><td><p>No → Reject</p><p>Yes → proceed to Stage 2</p></td></tr><tr><td>2</td><td>Market Availability </td><td>Is the token available in both Spot and Perpetual Futures on Binance?</td><td>Yes → Accept<br>Only Spot or Only Futures → proceed to Stage 3<br>Neither → Reject</td></tr><tr><td>3</td><td>Cross‑Exchange Verification</td><td>Is the token listed on Top‑10 CEXs or leading DEXs with verifiable depth and non‑synthetic volume?</td><td>Yes → Accept<br>No → Reject</td></tr></tbody></table>

Tokens that pass all three stages are classified as eligible collateral and can be accepted on Falcon Finance.

### Quantitative Risk Assessment

Each token is scored across four market‑quality dimensions.&#x20;

A color‑coded tier (🟢 Low, 🟡 Medium, 🔴 High) is assigned per factor.

<table><thead><tr><th width="255.92578125">Risk Factor</th><th>Low Risk 🟢 </th><th>Medium Risk 🟡 </th><th>High Risk 🔴</th></tr></thead><tbody><tr><td>Liquidity on Binance<br>- Daily Spot + Futures volume</td><td>More than USD 5M</td><td>USD 1M - 5M</td><td>Less than USD 1M or only illiquid pairs </td></tr><tr><td>Funding Rate Stability</td><td><ul><li>Consistently positive/neutral</li><li> Minimal spikes</li></ul></td><td><ul><li>Occasional negative<br>or spiky funding</li><li>Slight<br>inconsistencies</li></ul></td><td><ul><li>Highly negative or<br>volatile funding rates</li><li>Historically unstable</li></ul></td></tr><tr><td>Open Interest </td><td>Stable and high Open<br>Interest (more than USD 5M),<br>indicating sustained trader<br>interest</td><td>Moderate Open Interest (USD 1M - 5M), with noticeable fluctuations</td><td>Low Open Interest<br>(less than USD 1M) or frequent<br>drops, with  sudden<br>wipe-outs</td></tr><tr><td>Market Data Sources</td><td><ul><li>Cross-listed on Top 10 CEXs &#x26; DEXs</li><li>Low slippage</li><li>Deep books and consistent volume</li></ul></td><td><ul><li>Listed on mid-tier<br>exchanges</li><li>Moderate<br>slippage</li><li>Lower depth</li></ul></td><td><ul><li>Illiquid DEX listings<br>only</li><li>Poor price<br>discovery</li><li>Lack of<br>external validation</li></ul></td></tr></tbody></table>

## Composite Risk Grade&#x20;

* An asset is **Eligible** when **no factor is rated 🔴** and ≤ one factor is 🟡.
* Assets with two 🟡 scores are **Conditionally Eligible** and may receive a **higher overcollaterization ratio**.
* Any 🔴 score triggers **Rejection** or immediate review if already listed.



## Overcollaterization Ratio

Falcon applies dynamic overcollaterization ratios that reflect the composite risk grade and underlying asset volatility. Specific ratios are published on the [Falcon Finance Mint page](https://app.falcon.finance/swap/mint) and may change as market conditions evolve.



