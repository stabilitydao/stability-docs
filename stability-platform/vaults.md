# Vaults

The DeFi vault is an asset management service that automatically optimizes the return on your contributed funds. Vaults aggregate user funds into pools, reducing overall transaction costs and optimising returns for each pool participant. Vault is [ERC-20](https://ethereum.org/en/developers/docs/standards/tokens/erc-20/) token.

Our universal vault implementations allow users to create and use a variety of vaults for different purposes.

## Vault types <a href="#vault-types-contract" id="vault-types-contract"></a>

### Compounding vault  ( **CVault ) :**&#x20;

Stability has a tokenised auto-compounding vault featuring a solitary underlying liquidity mining position. Noteworthy in its design, this vault orchestrates the automatic reinvestment of all generated income

Moreover, this feature significantly enhances the potential for wealth growth. By consistently reinvesting generated income, the tokenised vault maximises compounding benefits, contributing to sustained and optimised returns for depositors. Stability not only prioritises user ease but also aims to empower individuals with a passive yet robust strategy for wealth accumulation in the dynamic landscape of decentralised finance.

### Rewarding vault ( RVault ):

RVault comes packed with perks – you get claimable rewards, a special buy-back token (BB-token), and initial boost rewards. Here's the deal: all the money we make is converted into BB-tokens for you. Plus, we make sure you get over $30 in boost rewards every day for the first 30 days. To keep things fair, we distribute the BB-token rewards over 7 days and the boost rewards over 30 days, so you can enjoy your gains at a steady pace. It's our way of making sure you have a smooth and rewarding journey with Stability.

Depending on the ratio, part of BB-token rewards is obtained by swapping into the BB-token, the other part is paid from the vault balance, which is received directly from the user creating the vault (project owner, market maker etc). In the second case, the earned assets themselves are sent to the owner of VaultManager NFT, which he can dispose of at his own discretion.

### Rewarding Managed Vault ( RMVault ):

{% hint style="info" %}
Coming soon
{% endhint %}

In addition to the functionality of the Rewarding vault, this one has additional capabilities that can be managed by the owner of the VaultManager NFT.

### Rewarding Investor-managed Vault ( RIMVault ):

{% hint style="info" %}
Coming soon
{% endhint %}

Vault users actively participate in on-chain voting processes to collectively make decisions regarding parameter changes.

### Splitter vault ( SVault ):

{% hint style="info" %}
Coming soon
{% endhint %}

SVault strategically allocates funds into a designated set of other vaults based on predefined proportions.
