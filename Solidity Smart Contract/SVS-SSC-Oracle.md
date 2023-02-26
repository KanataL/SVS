# Oracle

## Description
Oracle serves as a price feeder for projects

## Example Project

## Main functions/Components
- update cumulative price for the observation at the current timestamp
- consult the price

## Risk  Parmaters
- time interval (TWAP)
- Price feeder
- calculate price

## Threat Modeling
- Any potential read-only reentrancy attack vector?
- Are the time interval correctly set? (should more than 1 hour)
- Where is the reserve data from?
    - Any use of reserves in the pair?
    - Are the single source being used