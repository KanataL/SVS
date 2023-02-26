## Description

## Example Project

## Main functions/Components

## Risk Parameters

## Threat Modeling
- Any Front Running Attack vectors?
	- Any possibility for attackers to win the bid by front running the transaction?
- Any DoS Attack vectors?
	- Any possibility for attackers to prevent legitimate bids from being processed?
- Any Vulerability related to the sells strategies?
	- Dutch Auction/ Sealed bid
		- Are the corresponding variables correctly updated for a higher bid?
		- Any DoS attacker vectors to prevent other users from biding with a new price?
	- English Auction
		- Who will finalize the auction?
		- How will the bid be choosen?
- Any possible input validation issues?
	- Can attacker gain approvals for spending others' tokens?
	- Can attacker inject malicious data from the input to drain assets?
- Is the pull-over-push pattern used when transfering, especially refunding ETH ?
- Any Reentrancy Attack vectors (for multiple functions)?