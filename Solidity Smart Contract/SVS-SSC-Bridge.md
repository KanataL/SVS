# Bridge

## Description
-   Centralized bridge  
    Crypto exchanges block the user's assets, and offer similar ones in other networks.
-   Decentralized Bridge  
    The bridge uses a smart contract that connects different networks.
-   Side Chain Bridge  
    Between the core network and the child network.

## Example Project

## Main functions/Components
-   Deposit()
-   Withdraw()
-   Set owner

## Risk  Parmaters
-   Signature
-   RootHash

## Threat Modeling

-   Are the correct event emitted?
-   Are necessary access control enforce when bridging assets?
-   Are the correct amount of assets being locked to the bridge when deposit?
- If signature is used for verification, following should be checked
	- Verify that bridge requires all necessary values to be included in the message and signed: chain ids, receiver, amount, nonce.
	- Verify that used signatures are invalidated to protect bridge from replay attacks.
	- Verify that message hash generation algorithm is resistant to collision attacks. For example, using of `abi.encodePacked`
	- Verify that bridge includes source and destination chains identifiers in the signed message and correctly verifies them.
	- Verify that bridge does not allow to spoof chain identifier.
	- Verify that bridge uses a nonce parameter to allow the same operation (the same sender, receiver and amount) to be executed multiple times.
	- Verify signed message cannot be used in a differenct context (use domain separator from EIP-712).