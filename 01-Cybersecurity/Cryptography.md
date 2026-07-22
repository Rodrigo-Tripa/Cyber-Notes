## Overview

Cryptography is the practice of protecting information by transforming it into a form that can only be understood by authorized parties. It is one of the fundamental technologies of cybersecurity and is used to provide confidentiality, integrity, authentication, and non-repudiation.

## Encryption

Encryption converts **plaintext** into **ciphertext** using a cryptographic algorithm and a key. Authorized users can recover the original information through **decryption**, while unauthorized parties cannot interpret the encrypted data without the correct key.

### Symmetric Encryption

Symmetric encryption uses the same key for both encryption and decryption. It is fast and efficient, making it suitable for encrypting large amounts of data, but it requires a secure method of sharing the secret key.

### Asymmetric Encryption

Asymmetric encryption uses a pair of mathematically related keys: a **public key** for encryption and a **private key** for decryption. Although slower than symmetric encryption, it enables secure key exchange, authentication, and digital signatures.

## Hashing

Hashing is a one-way cryptographic process that transforms data into a fixed-length value known as a hash. Because hashing is irreversible, it is commonly used to verify data integrity, store passwords securely, and detect unauthorized modifications.

## Digital Signatures

Digital signatures use asymmetric cryptography to verify the authenticity and integrity of data. They allow recipients to confirm that information was created by the expected sender and has not been modified during transmission.

## Key Management

The security of any cryptographic system depends on protecting its cryptographic keys. Secure key generation, storage, distribution, rotation, and revocation are essential to prevent attackers from compromising encrypted data.

## Common Applications

Modern cryptography is used in technologies such as **HTTPS**, **TLS**, **SSH**, **VPNs**, secure messaging applications, password managers, digital certificates, and encrypted storage systems.