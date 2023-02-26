# Staking

## Description
Allow users deposit (LP) tokens into it and earn rewards in return.
- Timelock Liquidity Staking
- Masterchef-like staking

## Example Project

## Main functions/Components


## Risk  Parmaters

## Threat Modeling
- Any possible attack vector to steal locked funds from the contract?
- Reward Distribution
    - Does the Economy model resistant to flashloan attack/Whales
    - Will the truncation in math operations cause users/projects loss? (e.g., leftover in contract)
- Any corner cases should be addressed? (i.e., staking token is the same as reward token)
- Any possibility to set the staking tokens as reward to rugpull?
- Are the staking time being addressed?