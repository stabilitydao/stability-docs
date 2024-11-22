---
description: 'Last Update: November 2024'
---

# Vaults

The DeFi vault is an asset management service that automatically optimizes the return on your contributed funds. Vaults
aggregate user funds into pools, reducing overall transaction costs and optimising returns for each pool participant.
Vault is [ERC-20](https://ethereum.org/en/developers/docs/standards/tokens/erc-20/) token.

## Types

| Type                          | Description                                          | DefiLlama category (tvl)                                                         | Refs (tvl)                                                                                             | Our implementation      |
|-------------------------------|------------------------------------------------------|----------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------|-------------------------|
| [Compounder](./compounder.md) | Vault which re-invests income with single underlying | [Yield Aggregator](https://defillama.com/protocols/Yield%20Aggregator) ($3.2b)   | Beefy ($294m), Yearn ($228m)                                                                           | CVault.sol              |
| Harvester                     | Yield transport, yield tokenizer, boost aggregator   | [Yield](https://defillama.com/protocols/Yield) ($8.1b)                           | Pendle ($3.6b), Convex ($1b), Concentrator ($22m)                                                      | RVault.sol, RMVault.sol |
| ALM                           | Automated liquidity management vault                 | [Liquidity manager](https://defillama.com/protocols/Liquidity%20manager) ($550m) | Gamma ($54m), Ichi ($30m), Steer ($10m)                                                                |                         |
| Leverage                      | Vaults that increase position size using leverage    | [Leveraged Farming](https://defillama.com/protocols/Leveraged%20Farming) ($534m) | Extra ($160m), Gearbox ($96m), Alpaca ($34m)                                                           |                         |
| Portfolio                     | Multiple strategy assets in managed proportions      | [Indexes](https://defillama.com/protocols/Indexes) ($865m)                       | Enzyme ($194m), dHEDGE ($125m), Somm ($57m), Set ($70m)                                                |                         |
| [MetaVault](./metavault.md)   | AI-driven dynamic assets allocation                  | -                                                                                | [Singularity](https://docs.singularitydao.ai/) ($1.5m), [Mozaic](https://docs.mozaic.finance/) ($368k) |                         |
| OmniVault                     | Cross-chain vault                                    | -                                                                                |                                                                                                        |                         |