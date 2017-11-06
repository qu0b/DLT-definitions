# DLT-definitions
## address
## public key
## private key


## Proof of Stake
'In a PoS system, a blockchain **appends** and **agrees** on new blocks through a process where **anyone who holds coins** inside of the system can participate, and the **influence** an agent has is **proportional** to the number of coins (or “stake”) it holds' - [1]
### Chain-based proof of stake
"mimics proof of work mechanics and features a chain of blocks and simulates mining by pseudorandomly assigning the right to create new blocks to stakeholders." - [1]
### Byzantine fault tolerant (BFT) proof of stake.
conflicting (false) nodes cannot be created as long as 2/3 of the nodes follow the protocol honestly.
#### Block hash
computed by hashing the header, validation and transaction hashes. The block hash is also a merkle root. Any component of the block and account state can be verified with a merkle hash trail. "The block is valid if all the transactions in the block are valid adnd sufficient signatures are included in the validation" [1]. 
#### Validators
coins are held in a bond deposit. This is done by posting a **bond transaction**. Cryptographic signature known as votes are broadcasted to vote for the next block. **unbonding transaction** can be sent to unlock the coins. After the **unbonding transaction** an **unbonding period** (Short period of time) has to be waited before the coins can be spent.

#### Voting power
proportional to the bonded coins (coins at stake).

#### State hash
Included in the header. A merkle root hash of the persistent account hash.


### Nothing at stake
When someone has nothing to lose when contributing to a blockchain fork
## Proof of Work
## Block reversions

## Proposal mechanism
this is the mechanism that proposes blocks. Serves a similar role as the common abstraction of "leader election" used in traditional BFT algorithms.

## Friendly Finality Gadget
overlay ontop of a proposal mechanism

## Citations
[1] Casper the friendly finality gadget, Vitalik Buterin and Virgil Griffith, Ethereum Foundation, 17.10.17.
