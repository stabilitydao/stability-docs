---
description: >-
  This illustrated tutorial will guide you through each stage of adding funds to
  a Vault.
---

# Vault deposit

{% hint style="info" %}
Last Update: March 2024. Due to ongoing development, the interface you encounter may differ somewhat from the screenshots provided, as updates are continuously made.
{% endhint %}

## Prerequisites

* Your wallet needs to contain the vault's specific token(s). Learn how to add funds to your wallet here: [Replenish your wallet](../../onboarding/replenish-your-wallet.md)

## Walkthrough

### 1. Go to the [Stability Farm](https://stability.farm/) DApp page:

<figure><img src="../../.gitbook/assets/Screenshot 2024-03-08 at 13.37.38.png" alt=""><figcaption></figcaption></figure>

Ensure once more that our wallet is connected and that it is supplied with tokens.

### 2. Apply the filters to locate a vault you wish to make a deposit into:

<figure><img src="../../.gitbook/assets/Screenshot 2024-03-08 at 13.40.24.png" alt=""><figcaption></figcaption></figure>

### 3. Filter usage

<figure><img src="../../.gitbook/assets/Screenshot 2024-03-08 at 14.25.01.png" alt=""><figcaption></figcaption></figure>

In example we choose USDC asset and also pick Compound strategy to find corresponding vault. Open the Compound (CF) vault by clicking anywhere in the field.

### 4. Inside Compound vault

<figure><img src="../../.gitbook/assets/Screenshot 2024-03-08 at 14.28.58.png" alt=""><figcaption></figcaption></figure>

There is a lot of information inside the vault, such as TVL (Total Value Locked), Share Price and APR historical rates.

### 4. Deposit module

<div align="left">

<figure><img src="../../.gitbook/assets/Screenshot 2024-03-08 at 14.33.07.png" alt="" width="375"><figcaption></figcaption></figure>

</div>

Compound vault already sees that we have 5 USDC available in our wallet. A deposit field and a "Max" button are used for entering the exact amount of USDC to deposit.

### 6. Deposit

<div align="left">

<figure><img src="../../.gitbook/assets/Screenshot 2024-03-08 at 14.36.58.png" alt="" width="375"><figcaption></figcaption></figure>

</div>

In that case, we click the "Max" button to deposit all USDCs in our wallet.

Than, followed by clicking on the "Approve USDC.e" button to take an allowance for deposit.

In opened MetaMask pop-up window first make sure that our custom spending cap equals to requested allowance for deposit and than click "Approve" button.

<div>

<figure><img src="../../.gitbook/assets/Screenshot 2024-03-08 at 14.39.28.png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../../.gitbook/assets/Screenshot 2024-03-08 at 14.39.49.png" alt=""><figcaption></figcaption></figure>

</div>

Now "Deposit" button is available on module. Click on it and confirm transaction in our wallet.

<div align="left">

<figure><img src="../../.gitbook/assets/Screenshot 2024-03-08 at 14.42.30.png" alt="" width="375"><figcaption></figcaption></figure>

</div>

So now our deposit transaction succeed and we can check it on [Polygonscan](https://polygonscan.com/tx/0x24998e10d4ae884aa26ae79c0ff8e0a1d07a5a64b5f98f48cc81a5b089f06b9f) by clicking on corresponding button

<div align="left">

<figure><img src="../../.gitbook/assets/Screenshot 2024-03-08 at 14.52.37.png" alt="" width="309"><figcaption></figcaption></figure>

</div>

<figure><img src="../../.gitbook/assets/Screenshot 2024-03-08 at 14.49.27.png" alt=""><figcaption></figcaption></figure>

On a dashboard TVL amount was increased by 5 USDC and now our vault balance equals 5 USDC

<figure><img src="../../.gitbook/assets/Screenshot 2024-03-08 at 14.50.12.png" alt=""><figcaption></figcaption></figure>

In summary, depositing into a new vault always requires two transactions: one for approving the spending permission and one for the actual deposit.

Once the Hardwork function is called on this vault, you are already earning yield!

That's it.
