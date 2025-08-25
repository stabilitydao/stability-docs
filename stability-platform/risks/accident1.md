---
description: 'Last Update: Aug 25, 2025'
---

# Accident 1: Credix rugpull

## What is Credix?

Credix was a lending protocol in Sonic, running on Aave 3.0.2 codebase, which was used in our MetaVaults to allocate
some of the funds. A due diligence was carried out and protocol owners were KyCed.

## Rugpull

On July 29, 2025, Credix multisig executed
batch [transaction](https://sonicscan.org/tx/0x0cc3520951a2b41281dcc9a0d37ef3f7f139b75675d83ae72e3b8e903334f35e) with
granting all protocol roles to EOA `0xF321683831Be16eeD74dfA58b02a37483cEC662e`. On August 4, 2025, this address minted
unbacked collateral tokens using bridge
role [tx](https://sonicscan.org/tx/0x5db25b5c423dafd620d326e8765b160bafacfeaab2fecbb1d239c72dfeee4fa5) and drained (
borrowed) all available liquidity from protocol.

## Compensation

Stability DAO has committed to covering the financial damages caused by this accident to all affected users of our Meta
Vaults. Compensation is provided to all holders of MetaVaults and WrappedMetaVaults, as well as to all users of
protocols whose contracts were working with MetaVaults or WrappedMetaVaults at the time of the accident.

Until full compensation is achieved, we allocate 20% of the platform's income to it. We are engaging with police
authorities as well to recover the funds.

Compensation begin in Sep, 2025.

Compensation occurs to the liquid recovery tokens holders.

## Recovery tokens

All accident affected funds tokenized in Recovery tokens.

| Vault                                                                                  | Recovery token                                                                                                         | Initial supply |
|----------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------|----------------|
| [metaUSD](https://sonicscan.org/address/0x1111111199558661Bf7Ff27b4F1623dC6b91Aa3e)    | [0x000078392f3cF4262500FFeB7d803F90477ECC11](https://sonicscan.org/address/0x000078392f3cf4262500ffeb7d803f90477ecc11) | 300,968 USD    |
| [wmetaUSD](https://sonicscan.org/address/0xAaAaaAAac311D0572Bffb4772fe985A750E88805)   | [0x00001b2c60cD041a478521008CE6efeC475bb9Aa](https://sonicscan.org/address/0x00001b2c60cd041a478521008ce6efec475bb9aa) | 1,572,889 USD  |
| [wmetaUSDC](https://sonicscan.org/address/0xEEEEEEE6d95E55A468D32FeB5d6648754d10A967)  | [0x0000a59C549b4250a2931ac6054e1426a87DA0EE](https://sonicscan.org/address/0x0000a59c549b4250a2931ac6054e1426a87da0ee) | 105,768 USD    |
| [wmetascUSD](https://sonicscan.org/address/0xccccCCcca9FC69a2b32408730011EdB3205A93A1) | [0x0000c3b22bbD290588361E4B5C424F3AB0d0a3cc](https://sonicscan.org/address/0x0000c3b22bbd290588361e4b5c424f3ab0d0a3cc) | 1,042,155 USD  |
| [metaS](https://sonicscan.org/address/0x4444444420D9De54d69b3997b7D6A31d2BF63F32)      | [0x000006539BA0B4f5452186Af40aAB959bDEa4344](https://sonicscan.org/address/0x000006539ba0b4f5452186af40aab959bdea4344) | 1,099,758 S    |
| [wmetaS](https://sonicscan.org/address/0xbbbbbbBBbd0aE69510cE374A86749f8276647B19)     | [0x0000Dd8cEa00EA3336f5849590d69bbfc93A85bb](https://sonicscan.org/address/0x0000dd8cea00ea3336f5849590d69bbfc93a85bb) | 3,168,520 S    |

## Affected protocols users

For affected pools users we distributing recovery tokens by pool snapshots.

| Protocol                                                                                                                                                                                                                            | Contract                                                                                                               | Snapshot                                                                                                                           | Supply                   |
|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------|--------------------------|
| [Silo V2 market 125 wmetaUSDC-scUSD](https://v2.silo.finance/markets/sonic/wmetausd-scusd-125?action=information)                                                                                                                   | [0x6e8C150224D6e9B646889b96EFF6f7FD742e2C22](https://sonicscan.org/address/0x6e8c150224d6e9b646889b96eff6f7fd742e2c22) |                                                                                                                                    | 904,723 RECwmetaUSD      |
| [Silo V2 market 121](https://v2.silo.finance/markets/sonic/wmetausd-usdc-121?action=information)                                                                                                                                    | [0xCCdDbBbd1E36a6EDA3a84CdCee2040A86225Ba71](https://sonicscan.org/address/0xccddbbbd1e36a6eda3a84cdcee2040a86225ba71) |                                                                                                                                    | 380,298 RECwmetaUSD      |
| [Stability wmetaUSD-USDC](https://stability.market/?market=wmetaUSD)                                                                                                                                                                | [0x287939376DCc571b5ee699DD8E72199989424A2E](https://sonicscan.org/address/0x287939376dcc571b5ee699dd8e72199989424a2e) |                                                                                                                                    | 255,586 RECwmetaUSD      |
| Ichi SwapX wmetaUSD-wstkscUSD                                                                                                                                                                                                       | [0x859C08DDB344FaCf01027FE7e75C5DFA6230c7dE](https://sonicscan.org/address/0x859c08ddb344facf01027fe7e75c5dfa6230c7de) |                                                                                                                                    | 	21,557 RECwmetaUSD      |
| Euler wmetaUSD                                                                                                                                                                                                                      | [0x6F11663766bB213003cD74EB09ff4c67145023c5](https://sonicscan.org/address/0x6f11663766bb213003cd74eb09ff4c67145023c5) |                                                                                                                                    | 7,593 RECwmetaUSD        |
| Beets V3 [Stably Ever After: The Meta Mix](https://beets.fi/pools/sonic/v3/0x5103ea917605463fc497396ba89d6732ce4b2d70) | [0xbA1333333333a1BA1108E8412f11850A5C319bA9](https://sonicscan.org/address/0xba1333333333a1ba1108e8412f11850a5c319ba9) | [41 users](https://docs.google.com/spreadsheets/d/1KYo1kX2_xF3d5QfGgQN3-y-D5WSHExG_5YZnD2NJbbw/edit?gid=1751475199#gid=1751475199) | 11,060 e6 RECwmetaUSDC   |
| Beets V3 [Stably Ever After: The Meta Mix](https://beets.fi/pools/sonic/v3/0x5103ea917605463fc497396ba89d6732ce4b2d70) and [Green Shoots, Stable Loots](https://beets.fi/pools/sonic/v3/0x5d177938870ff8cf9004af5c3248039c721dbf2a) | [0xbA1333333333a1BA1108E8412f11850A5C319bA9](https://sonicscan.org/address/0xba1333333333a1ba1108e8412f11850a5c319ba9) | [44 users](https://docs.google.com/spreadsheets/d/1KYo1kX2_xF3d5QfGgQN3-y-D5WSHExG_5YZnD2NJbbw/edit?gid=0#gid=0) | 143,756 e6 RECwmetascUSD |
| Euler wmetaS                                                                                                                                                                                                                        | [0xC37fa1c70D77bdEd373C551a92bAbcee44a9d04E](https://sonicscan.org/address/0xc37fa1c70d77bded373c551a92babcee44a9d04e) |                                                                                                                                    | 2,120,455 RECwmetaS      |
| [Silo V2 market 128 wmetaS-S](https://v2.silo.finance/markets/sonic/wmetas-s-128?action=information)                                                                                                                                | [0x1c1791911483E98875D162355feC47f37613f0FB](https://sonicscan.org/address/0x1c1791911483e98875d162355fec47f37613f0fb) |                                                                                                                                    | 997,722 RECwmetaS        |
| SwapX wmetaS-stS                                                                                                                                                                                                                    | [0xD58f0042811A2Af932d8eA2D7466123ce9052Cde](https://sonicscan.org/address/0xd58f0042811a2af932d8ea2d7466123ce9052cde) |                                                                                                                                    | 30,260 RECwmetaS         |

