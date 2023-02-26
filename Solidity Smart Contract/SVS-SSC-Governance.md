# Governance

## Description
A blockchain governance system is a rule-based decision-making process. It allows the community to suggest, discuss and implement changes and improvements. 

## Example Project

## Main functions/Components
- Create proposal
- Reviewing period(Depositing period)
    - cancel proposal
    - collect deposits(if applicable)
- Voting period
    - Vote yes/no
- Tallying
    - “rejected” or “passed ” or “reject with veto”
- Cancel/Execute Proposal

## Risk Parameters
- Time interval between voting process
- Voting power
- `quorumVotes`
- `proposalThreshold`

## Threat Modeling
- Any implementation issue that can cause the governance token has unlimited voting power?
    - Any double voting by the same address?
    - Are votes cleared when voting power is removed?
    - Is the delegated voting power removed by undelegate?
- Are voting power able to be reused for different proposals?
- Are proposals finalized after tallying
- What is the thresholds for choosing propoer/voting
    - Are the governance token be borrow or flashloaned?
- What is timelock/delay between the governance process?

## Related Incidents/Exploits