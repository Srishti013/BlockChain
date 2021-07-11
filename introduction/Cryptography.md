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
