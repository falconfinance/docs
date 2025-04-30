---
hidden: true
---

# Locked Positions

Locked Positions are a representation of users' non-stablecoin assets that have been locked as collateral to mint USDf. These will be displayed under the Locked Positions section within users' Falcon Account Overview.

### Example

<figure><img src="../../../../../.gitbook/assets/Screenshot 2025-04-08 at 11.57.18 AM.png" alt="" width="563"><figcaption></figcaption></figure>

In the image provided above, a user has a Locked Position with the following details:

* Asset: ETH
* Amount: 500 ETH
* Initial Mark Price: $1,580.39 per ETH
* Overcollateralization Ratio (OCR): 5%
* Overcollateralization Ratio (OCR) Buffer Amount: 25 ETH
* USDf Minted: 750,685.9691 USDf

The terms above and their respective values are defined and calculated as such:

**Overcollateralization Ratio (OCR)**\
An Overcollateralization Ratio (OCR) is set to indicate a user's total value of locked collateral relative to the amount of minted USDf.&#x20;

$$
\text{OCR} = \frac{\text{Initial Mark Price of Collateral} \times \text{Collateral Amount}}{\text{USDf Minted}}
$$

Using the example scenario, the user's USDf minted amount is calculated as:&#x20;

$$
\text{USDf Minted} = 500 \times 1580.39 \times 0.05 = 750,685.9691
$$

**Overcollateralization Ratio (OCR) Buffer Amount**&#x20;

OCR Buffer Amount is the portion of collateral retained by Falcon beyond the value of minted USDf. The buffer serves as a risk mitigation mechanism to safeguard the protocol against market fluctuations.&#x20;



The amount of collateral asset held as an OCR buffer should be equivalent to OCR \* total amount of total collateral locked

**USDf Minted**

The USDf Minted value represents the total amount of USDf minted to the users' connected wallet by locking non-stablecoin collateral (e.g. ETH). This figure reflects the borrowing capacity granted to you based on the protocol’s Overcollateralization Ratio (OCR) rules.

To fully unwind your position and reclaim your locked collateral, you are required to repay the exact amount of USDf minted, in this case - 750,685.9691 USDf.

Once the USDf has been successfully repaid, the corresponding collateral (e.g. 500 ETH) will be unlocked and returned to your Falcon Account.
