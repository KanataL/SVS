# Dex

## Description
Allows users to exchange crypto assets peer-to-peer. Transactions can occur either via a decentralized order book or by matching orders and setting prices algorithmically.
- StableSwap
- UniSwap (xy=k)
- Decentalized orderbook

## Example Project

## Main functions/Components


## Risk Parameters

## Threat Modeling
- For Swap/Curve model:
    - **Arbitrage risk** (i.e., Can attackers exploit burn/mint/swap functions to drain assets from pool? )
    - **Invariant check** (i.e., Is invariant checked before reserves are updated? )
- For Flashloan Feature:
    - **Repay check:** Are borrowed flashloan repaid at the end?
    - **Reentrancy guardrails:** Any reentrancy guardrail to avoid using flashloan to mint(add) liquidty?