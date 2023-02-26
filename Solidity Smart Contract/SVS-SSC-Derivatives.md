# Derivatives

## Description
The Perpetual Contract is similar to a traditional Futures Contract, but has a few differences.

Detailed Introduction and Funding Rate Calculations: https://www.bitmex.com/app/perpetualContractsGuide

## Example Project
- dydx
- GMX

## Main functions/Components
- Open Long/Short Position
- Increase Position
- Decrease Position
- Liquidate Long/Short Position
- Close Long/Short Position
- Create Stop-Loss/Take-Profit Order
- Update Stop-Loss/Take-Profit Order
- Execute Stop-Loss/Take-Profit Order

## Risk  Parmaters
- Maximum Leverage
- Funding Rate
- Interest Rate
- Funding Interval
- Mark Price
- Unrealized/Realized PNL (Profit and Loss)

## Threat Modeling
- Any protection to prevent whale manipulators?(set proper threshold for maxGlobalLongSize/maxGlobalShortSize) 
https://twitter.com/joshua_j_lim/status/1571554171395923968
- Any incorrect calculation of funding rate?