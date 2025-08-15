---
description: 'Last Update: Aug 15, 2025'
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
| [metaUSD](https://sonicscan.org/address/0x1111111199558661Bf7Ff27b4F1623dC6b91Aa3e)    | [0x000078392f3cF4262500FFeB7d803F90477ECC11](https://sonicscan.org/address/0x000078392f3cf4262500ffeb7d803f90477ecc11) | 300,968        |
| [wmetaUSD](https://sonicscan.org/address/0xAaAaaAAac311D0572Bffb4772fe985A750E88805)   | [0x00001b2c60cD041a478521008CE6efeC475bb9Aa](https://sonicscan.org/address/0x00001b2c60cd041a478521008ce6efec475bb9aa) | 1,572,889      |
| [metaUSDC](https://sonicscan.org/address/0x22222222780038f8817b3dE825a070225e6d9874)   | -                                                                                                                      |                |
| [wmetaUSDC](https://sonicscan.org/address/0xEEEEEEE6d95E55A468D32FeB5d6648754d10A967)  | [0x0000a59C549b4250a2931ac6054e1426a87DA0EE](https://sonicscan.org/address/0x0000a59c549b4250a2931ac6054e1426a87da0ee) | 105,768        |
| [metascUSD](https://sonicscan.org/address/0x33333333C480194b5B651987b7D00B20dDCbd287)  | -                                                                                                                      |                |
| [wmetascUSD](https://sonicscan.org/address/0xccccCCcca9FC69a2b32408730011EdB3205A93A1) | [0x0000c3b22bbD290588361E4B5C424F3AB0d0a3cc](https://sonicscan.org/address/0x0000c3b22bbd290588361e4b5c424f3ab0d0a3cc) | 1,042,155 S    |
| [metaS](https://sonicscan.org/address/0x4444444420D9De54d69b3997b7D6A31d2BF63F32)      | [0x000006539BA0B4f5452186Af40aAB959bDEa4344](https://sonicscan.org/address/0x000006539ba0b4f5452186af40aab959bdea4344) | 1,099,758 S    |
| [wmetaS](https://sonicscan.org/address/0xbbbbbbBBbd0aE69510cE374A86749f8276647B19)     | [0x0000Dd8cEa00EA3336f5849590d69bbfc93A85bb](https://sonicscan.org/address/0x0000dd8cea00ea3336f5849590d69bbfc93a85bb) | 3,168,520 S    |
| [metawS](https://sonicscan.org/address/0x555555554776B14B30597d1032E48f9e16db22A4)     | -                                                                                                                      |                |
| [wmetawS](https://sonicscan.org/address/0xffFFFFFf2fcBeFAe12F1372C56edC769BD411685)    | -                                                                                                                      |                |
