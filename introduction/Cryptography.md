# Cryptography

* Blockchain provides users with data integrity in a trustless environment.
* This is accomplished using cryptography in a way that moves the burden of trust from data processors to cryptographic algorithms.
* Key terms used in cryptography:
  - **Secret**: The data which we are trying to protect
  - **Key**: A piece of data used for encrypting and decrypting the secret
  - **Function**: The process or function used to encrypt the secret
  - **Cipher**: The encrypted secret data, the output of the function.
* Simple example function:
  - Secret = "Blockchain Training Alliance"
  - Function = Swap each letter in the secret with a new letter according to the Key
  - Key = "+2"
  - Cipher = "Dnqemejckp Vtckpcpi Cnnkcpeg".
  
* Blockchain makes use of several different types of cryptography. Among these are:
   - **Public Key Cryptography** :
     Using a person's public key, it is possible to encrypt a message so that only the person with the private key can decrypt and read it. Using a private key, a digital signature can be created so that anyone with the corresponding public key can verify that the message was created by the owner of the private key and was not modified since.
   - **Zero-Knowledge Proof**:
     Prove knowledge of a secret without revealing it.
    - **Hash Functions** :
      One-way pseudo-random mathematical functions and Merkle trees.

### Ethereum Vs Hyperlegder
* Ethereum and Hyperledger Fabric are two blockchain systems that are taking different approaches to moving business to the blockchain. 
* In both Ethereum and Hyperledger Fabric, blocks include the hash of the previous block to tie the blockchain into a cohesive whole.
* Both Ethereum and Hyperledger Fabric are smart contract platforms that use a particular type of Merkle tree called the Patricia tree to store the current state of their virtual machine.
* Ethereum currently uses Proof of Work for consensus, though a switch to Proof of Stake has been built into the road map from the beginning. There are only two consensus algorithms implemented in Hyperledger Fabric - Solo and Kafka. SOLO is for development and Kafka is for production. 
* In Ethereum, users are identified by an address that is directly related to the user's public key. This provides identity verification while preserving anonymity. In Hyperledger Fabric, users are identified via X.509 certificates. These certificates provide several pieces of information about the user, but one of these is also the user's public key.
* Ethereum does not have support for zero-knowledge proofs, but adding the necessary functionality for zkSNARKS, a type of zero-knowledge proof, is currently included in the Ethereum development roadmap. Hyperledger Fabric does not currently support zero-knowledge proofs as a privacy feature.
      
 
 ### Merkle Tree
* A special type of data storage structure based on hash functions is called a Merkle tree.
* The hash of one block is made using the hashes of all the transactions of the block(combining 2 at a time).
* It is structured as a binary tree; the leaves contain the values to be stored and each internal node is the hash of its two children.
* It provides efficient lookups and protection against forgery since verifying a transaction is included in the tree. Can be accomplished by sending only the transaction, the     hash contained in each node between the transaction leaf node and the root, and the hash values used to create each hash sent.
* Looking up a transaction in a Merkle tree with three levels includes sending two transactions (the desired one and the other child of its parent) and three hashes (the           transaction’s parent, the root, and the root’s other child).
 
 
 
