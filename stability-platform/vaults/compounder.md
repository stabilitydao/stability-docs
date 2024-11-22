---
description: 'Last Update: November 2024'
---

# Compounder vault

The Compounder is classic yield-farming auto-compounding vault with single underlying asset. It invests the holders' funds into a given pool (LP, lending, vault on another platform or something else), claims and utilizes all available rewards and reinvests the income into the same pool.

## Our implementation

Smart contract: [CVault.sol](https://github.com/stabilitydao/stability-contracts/blob/main/src/core/vaults/CVault.sol)

**CVault** is modern universal yield-bearing vault implementation with capabilities that are not available to most other compounders and ERC-4626 vaults.

### Unique features

* The starting price of 1.0 share of vault is equal to $1
* Returns the price trust status. Vault works with both spot prices and trusted prices from oracles.
* Built-in protection against all types of flash loan attacks
* Vault may not have an underlying token, allowing it to work by providing liquidity to CLAMM pools without third-party liquidity managers. That is, this vault may be an ALM.

### How it works

The logic of investing and processing income is implemented in the strategy contract that the vault uses. [Strategies](../strategies.md) need to be implemented for each unique protocol bundle.

The process of claiming, liquidating and reinvesting income, called **HardWork**, occurs at least once every 24 hours, if there are rewards in the pool. If the rewards that the strategy utilizes run out (usually rewards run out sooner or later), then HardWork is not performed.

