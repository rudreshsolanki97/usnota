# USNOTA Contract

Token & Proxy contract for USNOTA - stablcoin pegged to USD deployed on XDC blockchain.

Contract Address - [xdcd04275e2fd2875beaade6a80b39a75d4fe267df6](https://explorer.xinfin.network/addr/xdcd04275e2fd2875beaade6a80b39a75d4fe267df6#contractSource)


## Brief on Proxy

All the function calls are made to a proxy contract which delegates calls to the implementation. The context i.e. address where all data regarding the state of the contract is stored will be on Proxy contract and not on implementation contract.

This empowers us to change the contract functionality at a later stage after deployment. Storage collisions have been considered and the contract follows [EIP-1967: Standard Proxy Storage Slots](https://eips.ethereum.org/EIPS/eip-1967) for the same, so explorers can identify that the contract is a proxy.

## Audit

An internal audit has been done of the smart contract