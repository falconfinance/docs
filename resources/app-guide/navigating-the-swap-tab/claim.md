---
description: A Step-by-Step Guide for Using the Claim Function
---

# Claim

### **Overview**

The Claim sub-function under the Locked Positions section of the Falcon Account Overview allows users who have minted USDf with non-stablecoin assets to claim their locked positions. Users can claim their locked positions in the form of their initial deposit asset, USDT, or a combination of both.\
&#xNAN;_&#x54;his feature will be moved under the Swap tab in the future._

### User Flow for Claiming Locked Positions

**Step 1: Navigate to the Claim Section**\
First, users locate the Account tab on the Falcon App, and select Profile from its dropdown menu. Then locate the Claim button under Falcon Account and Locked Positions.

<figure><img src="../../../.gitbook/assets/image (65).png" alt="" width="375"><figcaption></figcaption></figure>

**Step 2: Select Locked Position to Claim**\
Users select the locked position that they intend to claim and click Claim.

**Step 3: Check for Sufficient USDf Balance**\
To claim their locked positions, users will require a USDf balance in their Falcon Account equivalent or greater than the amount of USDf initially minted with the locked position.\
Users who do not meet the indicated USDf balance will be required to either mint or deposit the USDf difference into their Falcon Account to claim their locked position.

<div align="center"><figure><img src="../../../.gitbook/assets/Screenshot 2025-04-20 at 11.14.56 PM copy.png" alt="" width="375"><figcaption></figcaption></figure></div>

<div align="center"><figure><img src="../../../.gitbook/assets/Screenshot 2025-04-20 at 11.14.56 PM.png" alt="" width="375"><figcaption></figcaption></figure></div>

**Step 4: Select Claim Asset**\
Once the required USDf value is met, users can indicate their preferred claim asset in which they wish to receive their locked position. Users are able to choose between three options:

* Initial collateral asset:&#x20;
  * Users receive the equivalent of their locked position's value (USDf minted + overcolleralization buffer) completely in their initial collateral asset.
* USDT:
  * Users receive the equivalent of their locked position's value completely in USDT.
* Initial collateral asset + USDT:
  * Users receive the equivalent of their locked position's value in a combination of their initial collateral asset and USDT.&#x20;
  * The amount of collateral asset that can be claimed will be equal to or less than the initial overcollateralization buffer. The amount of overcollateralization buffer a user can claim is determined by the prevailing market price at the time of claiming.&#x20;
    * If the market price exceeds the initial deposit price: The redeemable value of the buffer will be capped at the original USD value of the deposit.&#x20;
    * If the market price falls below the deposit price: Users may reclaim the full unit quantity of the buffer, calculated at the lower market price.
  * The amount of USDT claimed will be equivalent to the initial amount of USDf minted by the user.

Once selected, users can initiate the claim of their locked positions to their Falcon Account by clicking the Confirm Claim button, which triggers the claim transaction.&#x20;

<figure><img src="../../../.gitbook/assets/Screenshot 2025-04-20 at 11.01.52 PM (1).png" alt="" width="375"><figcaption><p><em>Chosen option: <strong>Non-stable coin</strong></em></p></figcaption></figure>

_Note:  The amounts and valuations shown in the image above are indicative. Final amount received may vary based on market conditions and the time of redemption as price changes._&#x20;

**Step 5: Approve Transaction**\
Users will be required to confirm and authorize the transaction within their Web3 wallet.

**Step 6: Confirm Claim via Falcon Account Overview**\
After the claim is finalized and the transaction is confirmed, users' claimed assets will automatically be deposited into their Falcon Account after the 7-day cooldown period. Users should confirm this under the Profile function located in the dropdown menu of the Account tab.

<figure><img src="../../../.gitbook/assets/image (73).png" alt="" width="563"><figcaption></figcaption></figure>

### Withdrawal

After verification of a successful redemption, users can withdraw their assets to their Web3 wallets.

Refer to the [Withdraw](claim.md#withdrawal) section under the [Transfer](../navigating-the-transfer-tab/) tab for further details.

{% content-ref url="../navigating-the-transfer-tab/withdraw.md" %}
[withdraw.md](../navigating-the-transfer-tab/withdraw.md)
{% endcontent-ref %}
