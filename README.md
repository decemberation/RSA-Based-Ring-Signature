# RSA-Based-Ring-Signature
Python implementation of Ring Signature based on RSA Algorithm

1) Ring Siganture
- Terminology: a set of possible signers is called a ring. We call the ring member
who produces the actual signature the signer and each of the other ring members
a non-signer.
- We assume that each possible signer is associated with a public key Pk that defines 
his signature scheme and specifies his verification key. The corresponding secret key is denoted by Sk.
- A ring signature scheme is defined by two pro cedures:
  + ring-sign( m, P1, P2, . . . , Pr, s, Ss) which produces a ring signature σ for the
  message m, given the public keys P1, P2, . . . , Pr of the r ring members,
  together with the secret key Ss of the s-th member (who is the actual signer).
  + ring-verify(m, σ) which accepts a message m and a signature σ (which
  includes the public keys of all the possible signers), and outputs either true
  or false
  
2) Proposed signature scheme (RSA-based)
- RSA Trap-Door Permutations:
  ![image](https://user-images.githubusercontent.com/48883241/203467239-3ca18f72-8c5d-4d6b-9bab-b14e54a118d0.png)

- Hash Function: (SHA-256 was used)

- Combining Function:
  ![image](https://user-images.githubusercontent.com/48883241/203467147-a614a00f-ca71-4dc3-a565-1d98ea1a02e3.png)
  ![image](https://user-images.githubusercontent.com/48883241/203467159-fc4de4f1-bdfd-472e-8459-6b66966a8b86.png)





