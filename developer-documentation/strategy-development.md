---
description: >-
  Development of DeFi strategy logic is not simple. You need to understand how
  it all works.
---

# Strategy Development

## Prepare

Read [Core Developer's guide](https://github.com/stabilitydao/stability-contracts/blob/main/src/core/README.md) and read source code of existing strategies.

See [open STRATEGY issues](https://github.com/stabilitydao/stability-platform-contracts/issues?q=is%3Aopen+is%3Aissue+label%3ASTRATEGY), ask Stability team to asign you to any PROPOSED strategy and mark that strategy being developed.

Study the protocols used in the strategy. Conduct all interactions with protocols manually, or find links to such transactions in an explorer.

If you are stabilitydao member then Create branch from issue by Create a branch link, or just fork repo if not.

### 1. Create integration interfaces

Put third-party interfaces to `src/integrations/<protocol>/`.

### 2. Create constants

* Put your new strategy ID to `src/strategies/libs/StrategyIdLib.sol`
* Put your developer address to `src/strategies/libs/StrategyDeveloperLib.sol`
* Put the addresses necessary for the strategy to `chains/<ChainName>Lib.sol` constants (tokens, pools, addresses for interactions)

From now on you can already create draft Pull Request for merging to main branch of this repo.

### 3. Add swapper routes

For each token in strategy assets and farming reward assets the swapper must have a route. Add routes to `chains/<ChainName>Lib.sol` inside one of `routes*()` methods.

Also add swap thresholds for tokens to `runDeploy` method. Threshold value must be more then $0.0001 usually. If a token is supposed to be swapped for WBTC, which has 8 decimals, then the minimum is $0.001.

### 4. (Optional) Add farms

For farming strategy you need to add farming data to `chains/<ChainName>Lib.sol`.

The farm must contain a minimum amount of data to initialise the strategy, but rewardAssets are required, pool for LPStrategy is required too.

### 5. Implement strategy logic skeleton

Depending on the purpose of the logic, the strategy is inherited from a set of base classes:

* LPStrategyBase if strategy uses AMM
* FarmingStrategyBase if it is farming strategy

Put your strategy to `src/strategies/<YourStrategyContractName>.sol` and implement all functions that need for compiling.

Add your strategy logic deployment to `script/libs/DeployStrategyLib.sol` and to `runDeploy` method in `chains/<ChainName>Lib.sol`.

### 6. Add universal test

Put your test to `test/strategies/<YourStrategyContractName>.<ChainName>.t.sol` You must inherit from contracts `<ChainName>Setup`, `UniversalTest` and write `test***` method with adding strategy variations for testing by `strategies.push(...)`.

Run tests:

```bash
forge test -vv -match-test test***
```

### 7. Implement and debug strategy logic

Thanks to messages in the universal test, you can implement the logic of the strategy step by step. As a result, the test should be passed, and it should show APRs similar to real ones.

Check your strategy code size with `forge build --sizes` command. If your strategy size exceeds the permissible limit, then move part of the code to the library `src/strategies/libs/<YourStrategyContractName>Lib.sol`.

Mitigate security findings posted in PR.

### 8. Write deploy script

Put deploy script for operator to `script/DeployStrategy****.<ChainName>.s.sol` with deploying strategy implementation, adding swap routes and farms.

The script should not use `<ChainName>Lib.sol`, otherwise this lib will be deployed when the script is launched, which is unnecessary and is an extra waste of gas.

### 9. Finish

If the checks of the continuous integration system in your PR are passed, click 'Ready for review' button in your PR and request a review.

\
