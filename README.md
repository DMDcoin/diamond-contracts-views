# HbbftAggregator Contract

This Solidity contract aggregates data from various core contracts of the DMD chain into singular contract calls. It simplifies the retrieval of crucial data related to staking, validators, pools, and other related parameters.

## Interfaces

This contract interacts with the following interfaces:
- `IStakingHbbft`: For staking-related data.
- `IValidatorSetHbbft`: For validator set information.
- `ITxPermission`: For transaction permission data.
- `IKeyGenHistory`: For key generation history.
- `IBlockRewardHbbft`: For block reward information.

## Deployment Warning

⚠️ **Important**: The `HbbftAggregator` contract should be deployed **before** the other core contracts if you intend to fetch data from previous blocks. This ensures that the aggregator has access to the historical data necessary for accurate retrieval.

## Example Deployment Addresses

- **Staking Contract**: `0x1100000000000000000000000000000000000001`
- **ValidatorSet Contract**: `0x1000000000000000000000000000000000000001`
- **TxPermission Contract**: `0x4000000000000000000000000000000000000001`
