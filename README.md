# blockchain
Beers and Blockchains with Brandon

Watch me attempt to write a blockchain from scratch in python while sometimes drinking.


ontology of bitcoin:

Static components:
Block
  prev hash
  nonce
  merkle tree
Blockchain

Dynamic componenets:
NodeServer
  local blockchain
  scan for transactions
  broadcast transactions
  scan for blocks
  broadcast blocks
  mine block (proof-of-work)
  
Transactor
  public key
  send transactions to NodeServers


Paper: https://bitcoin.org/bitcoin.pdf
Paper outline:
1. Intro
2. Transactions
3. Timestamp Server
4. Proof-of-Work
5. Network
    1) New transactions are broadcast to all nodes.
    2) Each node collects new transactions into a block.
    3) Each node works on finding a difficult proof-of-work for its block.
    4) When a node finds a proof-of-work, it broadcasts the block to all nodes.
    5) Nodes accept the block only if all transactions in it are valid and not already spent.
    6) Nodes express their acceptance of the block by working on creating the next block in the
        chain, using the hash of the accepted block as the previous hash.
6. Incentive
7. Reclaiming Disk Space
8. Simplified Payment Verification
9. Combining and Splitting Value
10. Privacy
11. Calculations
12. Conclusion


LOG: 

----------------------------------------------------
01/22/2021

* wrote merkle tree class

----------------------------------------------------
01/24/2021

*inclusion proof
  *fixed merkle tree class
  *added parents to nodes
  *created repo




