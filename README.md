
# Truflation contest details

- Join [Sherlock Discord](https://discord.gg/MABEWyASkp)
- Submit findings using the issue page in your private contest repo (label issues as med or high)
- [Read for more details](https://docs.sherlock.xyz/audits/watsons)

# Q&A

### Q: On what chains are the smart contracts going to be deployed?
Trfulation Token, vesting, ve token, virtual staking rewards contract will be deployed on Base Mainnet.

The TruflationTokenCCIP is a ccip bridged token, and it will be deployed on other EVM networks including Ethereum Mainnet, Aribtrum, Optimism, Bnb, Polygon, Fantom
___

### Q: Which ERC20 tokens do you expect will interact with the smart contracts? 
They don't interact with other ERC20 tokens, just use TRUF ERC20 token.
___

### Q: Which ERC721 tokens do you expect will interact with the smart contracts? 
None
___

### Q: Do you plan to support ERC1155?
No
___

### Q: Which ERC777 tokens do you expect will interact with the smart contracts? 
None
___

### Q: Are there any FEE-ON-TRANSFER tokens interacting with the smart contracts?

No
___

### Q: Are there any REBASING tokens interacting with the smart contracts?

No
___

### Q: Are the admins of the protocols your contracts integrate with (if any) TRUSTED or RESTRICTED?
TRUSTED
___

### Q: Is the admin/owner of the protocol/contracts TRUSTED or RESTRICTED?
TRUSTED
___

### Q: Are there any additional protocol roles? If yes, please explain in detail:
TruflationTokenCCIP has ccipPool role, and it allows to mint and burn tokens.
___

### Q: Is the code/contract expected to comply with any EIPs? Are there specific assumptions around adhering to those EIPs that Watsons should be aware of?
TruflationToken is complies EIP-677 like LINK token.
___

### Q: Are there any off-chain mechanisms or off-chain procedures for the protocol (keeper bots, input validation expectations, etc)?
We need to use merkle tree for token migration.
TrufMigrator.sol is using this to allow users to claim TRUF tokens from snapshot.
___

### Q: In case of external protocol integrations, are the risks of external contracts pausing or executing an emergency withdrawal acceptable? If not, Watsons will submit issues related to these situations that can harm your protocol's functionality.
No external protocol integration.
___

### Q: Do you expect to use any of the following tokens with non-standard behaviour with the smart contracts?
No
___



# Audit scope


[truflation-contracts @ ec0862848d9461f6d681e423865aab7ec0027923](https://github.com/truflation/truflation-contracts/tree/ec0862848d9461f6d681e423865aab7ec0027923)
- [truflation-contracts/src/staking/VirtualStakingRewards.sol](truflation-contracts/src/staking/VirtualStakingRewards.sol)
- [truflation-contracts/src/token/ERC677Token.sol](truflation-contracts/src/token/ERC677Token.sol)
- [truflation-contracts/src/token/TfiBurn.sol](truflation-contracts/src/token/TfiBurn.sol)
- [truflation-contracts/src/token/TrufMigrator.sol](truflation-contracts/src/token/TrufMigrator.sol)
- [truflation-contracts/src/token/TrufVesting.sol](truflation-contracts/src/token/TrufVesting.sol)
- [truflation-contracts/src/token/TruflationToken.sol](truflation-contracts/src/token/TruflationToken.sol)
- [truflation-contracts/src/token/TruflationTokenCCIP.sol](truflation-contracts/src/token/TruflationTokenCCIP.sol)
- [truflation-contracts/src/token/VotingEscrowTruf.sol](truflation-contracts/src/token/VotingEscrowTruf.sol)

