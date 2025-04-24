# Rewards Distribution

### Overview

<figure><img src=".gitbook/assets/Screenshot 2025-04-16 at 4.23.10 PM.png" alt="" width="563"><figcaption></figcaption></figure>

Falcon calculates and verifies yields generated daily across all of its strategies. The generated yields are used to mint new USDf. A portion of the newly minted USDf is deposited directly into Falcon's sUSDf ERC-4626 Vault, increasing the vault's existing sUSDf : USDf value over time. The rest of the newly minted USDf is staked into the vault as sUSDf, and allocated to users with Boosted Yield NFTs.

If a user is using Classic Yield, they receive USDf when they unstake their sUSDf. The amount they get is based on the current sUSDf-to-USDf value, which will already account for their share of total yield accrued.

On the other hand, users who have participated in Falcon's Boosted Yield unstake (claim) their locked positions, they receive the additional sUSDf that was staked on their behalf. This enables them to enjoy the boosted yield, on top of their initial locked amount of sUSDf. They can then unstake their sUSDf for classic yield as with any other user.\
&#xNAN;_&#x52;estaked and boosted sUSDf positions will receive additional sUSDf only at maturity._

### Calculation of Yield

At the end of each 24-hour cycle, Falcon calculates the total amount of yield generated within the period, before distributing them to USDf stakers following the formula below:

$$
\text{Yield per User} = \frac{\text{USDf Staked by User}}{\text{Total USDf Staked}} \times \text{Yield Distributed}
$$

### On-chain Tracking

By utilizing the ERC-4626 standard, Falcon ensures that the sUSDf-to-USDf rate remains fully transparent and verifiable on-chain. Users can do so via Etherscan by following the below process:

<figure><img src=".gitbook/assets/image (92).png" alt="" width="563"><figcaption></figcaption></figure>

1. Visit the sUSDf contract on Etherscan: https://etherscan.io/address/0xc8CF6D7991f15525488b2A83Df53468D682Ba4B0#readProxyContract
2. Scroll to "convertToAssets" and input 1000000000000000000 (represents 1 sUSDf).
3. Divide the result (i.e, 1020540451406678530) by 10^18 to verify the current sUSDf-to-USDf rate (i.e, 1.020540451406678530)

### Lock Window

To maintain accuracy and prevent complications (e.g., last-minute entries or exits distorting daily returns), Falcon implements a brief lock window, often during the 9:00–10:00 PM GMT+8 timeslot. Yield is finalized within that same timeslot, and interactions such as staking and unstaking may briefly be queued to avoid overlapping transactions that could incorrectly allocate or dilute the daily rewards.

Once calculation and yield distribution are complete, Falcon incorporates the final figure into the next APY update.

_Additionally, clients who redeem assets before the daily unlock process is fully completed will forfeit a portion of their daily yields._
