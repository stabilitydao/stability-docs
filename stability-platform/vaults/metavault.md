---
description: 'Last Update: Apr 2025'
---

# MetaVault

A MetaVault is a vault that invests in other vaults. Our implementation has a unique architecture that was developed to automate the management of decentralized finances based on the Stability platform.

## Requirements

* Safe to use with all Stability vaults (Compounder/MetaVault), any assets
* Rebase stablecoin (pegged to USD, S, ETH, BTC) for fast yield delivery
* Wrapped version to use in lendings
* ERC4626 single asset wrapper to use in boosted pools

## Vaults in development

* **metaUSD**: investing in all strategies with USD stablecoins (lend, LP, leverage, etc)
  * metaUSDC: supplying USDC to lending protocols
  * metascUSD: supplying scUSD to lending protocols
* **metaS**: investing in all strategies with S
* **metaETH**: investing in all strategies with ETH
* **metaBTC**: investing in all strategies with BTC
* tradeS: metaS + metaBTC trading by agent
* tradeBTC: metaUSD + metaBTC trading by agent
* portfolioXXX: basket of MetaVaults in fixed or dynamic proportions
