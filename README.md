# RSA_Encryption
Implementation of RSA Encryption Algorithm

## About RSA Encryption:
  <p> RSA is designed by Ron Rivest, Adi Shamir, and Leonard
Adleman in 1978. It is one of the best known public key
cryptosystems for key exchange or digital signatures or
encryption of blocks of data. RSA uses a variable size
    encryption block and a variable size key. </p>
  
## Algorithm (Pseudocode)

_Key Generation Procedure_
```
- Choose two distinct large random prime numbers p & q
such that p ≠ q.
- Compute n= p × q.
- Calculate: phi (n) = (p-1) (q-1).
- Choose an integer e such that 1<e<phi(n)
- Compute d to satisfy the congruence relation d × e = 1
mod phi (n); d is kept as private key exponent.
- The public key is (n, e) and the private key is (n, d).
Keep all the values d, p, q and phi secret.
```
_Encryption_
```
- Plaintext: P < n
- Ciphertext: C= Pe mod n
```
_Decryption_
```
- Ciphertext: C
- Plaintext: P=Cd mod n.
```
