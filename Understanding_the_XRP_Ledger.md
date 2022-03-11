# Caution: Work in Progress
This is an open source textbook in development.

# Understanding the XRP Ledger

## 1. Introduction
### XRP Ledger
### Assets and tokens
### Rippling and Pathing
### Transaction types

## 2. Consensus
The XRP Ledger is a specialized accounting application that manages and maintains the balances of XRP Ledger accounts.

Suppose the software was in no way connected to a network. You could run a copy of the XRP Ledger on your computer and your friend Alice could run an identical copy on her computer. When you make a transaction, you could share the transaction with Alice by printing it out, and she could enter the same transaction on her copy. In this way the two ledgers can be kept in sync with eachother and could be considered to be the same ledger.

Joining the software to the Internet allows us to automate this, but there is still a problem: What if not everyone agrees perfectly on which transaction happened when? And what happens when two conflicting transacitons are entered at the same time (e.g. Bob wishes to send his last 1 XRP to Alice and Claire at the same time, and creates and submits two different transactions to do this.)

To solve this "consensus" problem we use a byzantine fault tolerant consensus protocol called the Ripple Consensus Protocol.

### 2.1 Ripple Consensus Protocol
In the RCP each participant in consensus nominates a _candidate set_ of transactions to be included in the next ledger. Based on the votes of the others, each participant removes or includes certain contested transactions to their proposed set. Each round the threshold for inclusion is increased until 80% of participants agree on a single candidate set. At this point the transaction set is applied, the ledger is closed and voting proceeds for the next ledger. 

[See white paper](https://ripple.com/files/ripple_consensus_whitepaper.pdf)
[See video explanation](https://vimeo.com/64405422)

// code inclusions needed

### 2.2 Validators
Validators are rippled instances which are configured to actively participate in the consensus process. Each opinion about a candidate set is signed with the Validation private key and broadcast to the network as a _TMValidation_ message.

// code inclusions needed

### 2.3 Amendments and Rules
### 2.4 Determinism

## 3. Ledgers and Ledger Entries
### Merkel Trees
### Keylets
### SHAMap
### Views

## 4. Serialisation
### sfCodes and types

## 5. Transactions and Transactors
### Anatomy of a transaction
### Signatures and signing fields
### Application and metadata

## 6. Persistent Storage

## 7. Network
### Mesh network
### IP network
### Peering and billing

## 8. Memory

## 9. Pointers and pointer types

## 10. Locking and Job Queue

## 11. Testing Regime

## 12. Building and contributing code

