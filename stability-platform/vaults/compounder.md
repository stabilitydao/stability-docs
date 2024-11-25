---
description: 'Last Update: November 2024'
---

# Compounder vault

The Compounder is classic yield-farming auto-compounding vault with single underlying asset. It invests the holders' funds into a given pool (LP, lending, vault on another platform or something else), claims and utilizes all available rewards and reinvests the income into the same pool. Compounder vault platforms are called Yield Aggregators and Yield Optimizers.

## Why is it needed?

Vault automates investing and managing of the user's crypto assets, who only needs to deposit and withdraw funds. Thanks to this, the Vault user gets the following advantages over those who invest assets manually.

* No need to waste gas and time on claiming and recycling rewards
* Achieve high levels of compound interest by reinvesting income daily
* The real income of the vault is tracked by the platform, which eliminates errors in asset management
* Instead of working with each application that has a yield, you can do everything in one, comparing yields and managing your portfolio

## Refs

* Yearn (July 2020)
* Beefy (September 2020)
* Harvest (September 2020)
* [Yield Aggregator](https://defillama.com/protocols/Yield%20Aggregator)

## Our implementation

Smart contract: [CVault.sol](https://github.com/stabilitydao/stability-contracts/blob/main/src/core/vaults/CVault.sol)

**CVault** is modern universal yield-bearing vault implementation with capabilities that are not available to most other compounders and ERC-4626 vaults.

### Unique features

* The starting price of 1.0 share of vault is equal to $1
* Returns the price trust status. Vault works with both spot prices and trusted prices from oracles.
* Built-in protection against all types of flash loan attacks
* Vault may not have an underlying token, allowing it to work by providing liquidity to CLAMM pools without third-party liquidity managers. That is, this vault may be an ALM.

### Strategy

The logic of investing and processing income is implemented in the **strategy** contract that the vault uses. [Strategies](../strategies.md) need to be implemented for each unique protocol bundle.

### HardWork

The process of claiming, liquidating and reinvesting income, called **HardWork**, occurs at least once every 24 hours, if there are rewards in the pool. If the rewards that the strategy utilizes run out (usually rewards run out sooner or later), then HardWork is not performed.

