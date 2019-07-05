# BlockChain E-Vote

## This project aims to increase the trust that people can feel in EVMs

### This will be done in two ways

- Making it easier to verify that the votes were not tampered with.
- Making it easier to verify that the counting is genuine.

## There will be two separate data channels

- One will be a standard relational database of all valid voters, for fast querying.
- The other will be the the blockchain of all the cast votes, for immutability and verifiablity.

## The following steps will be taken to make this work

- The voters' crypto wallets will be linked to their voter ID by the EC.
- The voters will make a per-election secret key pass, which will be separate from the wallet key.
- When the voter goes to the EVM, the machine will first verify that they are a real voter.
- Next, their voter ID will be encrypted by the election key and will be used to verify that they haven't already voted.
- If everything goes smoothly, the voter will cast their vote and a new block will be made.
- This block will have the serial number of the EVM, the encrypted voter ID and the vote.
- Before adding to the blockchain, the voter will be asked to confirm that they voted.
- The voter can verify that their vote went to the correct party in the blockchain.
- Anyone can count the votes in the blockchain to make sure the counting is genuine.
- Counting will be done simultaneously to save time and power.
- Voters can verify that their vote is casted to the right party and  is not being tampered with, anytime after voting using their secret key pass.

## The steps that the voters will need to take

- They must register for a crypto wallet.
- They must register their wallet with their voter ID.
- They must take the necessary steps to keep their keys separate and secret.

## The steps that the EC will need to take

- They must make sure that only the voter's wallet is linked to their ID.
- They must make sure that the people know not to use their wallet keys as election keys, in case of a breach.
