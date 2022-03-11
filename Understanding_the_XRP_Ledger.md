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

### 2.1 Validators and Proposals

### 2.2 Amendments and Rules
### 2.3 Determinism

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

