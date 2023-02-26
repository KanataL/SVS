# Lending

## Description
The decentralized lending protocol allows users to lend or borrow cryptocurrency without interacting with a centralized intermediary. Some lending protocols also support yield farming and derivative trading.

## Example Project
- [CoffinBox](https://docs.google.com/document/d/1ZrRb7zq_SBSNXhLcDbwzLMqOWRH-x9sj-70q9WkxkqU/edit)
- [New Free DAO](https://docs.google.com/document/d/1jo1XnJQt74HTR4QUOxGxM12kmmc7KIRtY7d2NkQiQLg/edit)
- [Deus Finance](https://docs.google.com/document/d/1l0HOuQIznEE-QwMrIzmA0IJP7_ba5Sj-LiEL3Pbk-F0/)
- Ola Finance
- FEGtoken

## Main functions/Components
-   Lending:
    -   Staking
    -   Collateral management      
-   Borrowing 
    -   Loans approval
    -   Repayment
-   Liquidation
    -   Mechamnism: e.g. Auction
    -   Liquidity pools
    -   Reward & service fees
-   Token Management
-   Governance
-   Price Oracle

## Risk  Parmaters
- Deposit & Staking module
    - Native token price
    - Staking(Yield farming) reward
- Borrow & Repay module
    - Interest Rate
    - Collateral factor
    - Redemption rate
    - Borrow fee
- Collateral Liquidation module
    - Liquidation reward
- Governance module
    - Governance token price
    - Voting power

## Threat Modeling
- Oracle integration
    - **Price manipulation** (Does the price feeder have enough liquidity? )
    - **Price result queried from oracle** (Does the precision of the price, the price ratio (i.e., A/B or B/A) align with the calculation?)
    - **Prices updated**(Are the price up-to-date? Over how much time the price can be considered to be invalid？)
- Reentrancy attack vectors
    - Are **ERC677/ERC777** tokens used in the project?
    - Are **ERC721** tokens used as collateral/position tracker in the project?
    - Are there any **native token transfers**?
- Combination with assets
    - What is the underlying assets accepted for the projects?
    - Does the asset has incompatibility with project (e.g., USDC has 6 decimal while normal ERC20 has 18) ?
- Collateral and Debt Records
    - Are the **Debt records correctly updated** during the process
- Fees/Interest caluculations
    - Is there any precision loss that could lead to loss?
    - Is the calculation model align with the design?