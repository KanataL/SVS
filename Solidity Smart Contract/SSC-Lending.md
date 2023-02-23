# SSC: Lending
| #| Description |
| --- | --- |
| **1** | Verify that price is not calculated using the reserve price or centralized oracle feed. |
| **2** | Verify that the instant price is not used in price calculation. |
| **3** | Verify that the all price-related parameters are updated at the same time.  |
| **4** | Verify that all the sensitive value are correctly updated before and after some function executions: balance/reserve, price, reward, etc. |
| **5** | Verify that service fees, royalties and taxes are correctly included or excluded. |
| **6** | Verify that all fees or rewards calculation are isolated from unverified/abondend contracts. |
|**7**|Verify that the voting power of governance can be manipulated.|
|**8**| Verify that the if the sensitive calculation should be executed within one block or not. |
|**9**| Verify that the addiontional token mint/burn of following functions are correct: reward, rebase, deposit/withdraw, stake/unstaked, addLiquidity/removeLiquidity, etc.|
|**10**| Verify that the price slippage is carefully considered when adding/removing liquidity.|
