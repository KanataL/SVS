# Aggregator

## Description
Yield aggregators are a set of smart contracts that pool investors’ crypto assets (tokens) and invest them in a portfolio of yield-paying products and services through pre-programmed and automatically executed strategies.

## Example Project

## Main functions/Components
-   vault   
    -   deposit
    -   withdraw
    -   earn / farm
    -   add strategy
    -   remove strategy
-   startegy
    -   deposit
    -   withdraw
    -   harvest     
-   charge fee
-   Reward calculation
-   Token Swap

## Risk  Parmaters
-   shares
-   strategy 
-   fee

## Threat Modeling
-   Vault:
    -   Are the shares been correctly tracked 
    -   Are the yield been distributed based on shares?
    -   Can the rewards be inflated by flashloan?
    -   Any depositFor() function that can deposit tokens for others? 
    - Any issue related share transfer?   
    -  Any possibility to transfer shares? Any issue related share transfer?
        
-   Strategy:
    -   Is the strategy contract correctly reflect the target project logic
    -   Any potential attack vectors to steal funds from strategy contracts

- Reward logic
    - Will the reward logic vulnerable to flashloan attacks?
    - Will user lose reward due to calculation/logic
