# Security Workshop

## Who am I? 
My name is Anna! I’ve been interested in security since I was a kid. I’m currently an Undergraduate Research Assistant in the 
[Cryptography, Security and Privacy Lab (CrySP)](https://crysp.uwaterloo.ca/) working on [Slitheen](https://crysp.uwaterloo.ca/software/slitheen/), an 
anti-censorship system.

You can find me here:
- Twitter: @securitanna
- Website: www.annalorimer.com 

## Disclaimer
Security is a rich and nuanced field! So, we couldn’t possibly cover everything in this workshop. The goal of this workshop is to give you enough background to get started and to introduce you to a commonly used library. By no means does this workshop guarantee that by the end you will have the skills to implement cryptography correctly or guarantee vulnerability-free software. 

## What is security? 
- Security is about protecting assets 
  - Assets are things like data, hardware, software 
- How are assets harmed? 
  - Threats come in the form of vulnerabilities, denied access, modified and/or lost files, stolen hardware etc . 

## Cryptography!
- Crypto has been around since people needed to keep secrets
  - Ex. Caesar invented the Caesar Cipher to keep his troop movements secret
- Terminology:
  - Sender and receiver: The *sender* wants to send a message securely to the *receiver*
  - Plaintext: Unencrypted, unmodified messages
  - Ciphertext: The output of running an encryption algorithm on plaintext
  - Encryption: The process of disguising plaintext
  - Decryption: Converting ciphertext to plaintext
  - Cryptography: The science and art of keeping things secure
  - Cryptanalysis: the science and art of breaking ciphertext 
- Cryptography Characters
  - Ever heard of Alice and Bob? They’re possibly the most famous characters of cryptography. 
  - Cryptographic protocols and algorithms are often described using characters. 
  - Common characters:
    - Alice and Bob: Sender and Receiver
    - Eve: Eavesdropper (passive)
    - Mallory: Malicious attacker (active)
    - Trent: A trusted third party or arbitrator 
- Cryptographic Algorithms 
  - Symmetric
    - Algorithms that have the property that encryption keys can be derived from the decryption key and vice versa (Schneier)
    - One key is needed for the algorithm
    - Sender and Receiver must agree on a key before sharing any information
    - Ex. Caesar Cipher. The sender and receiver must agree on how the message is shifted before they can send messages. 
  - Asymmetric or Public Key
    - 2 keys: 1 for encryption and one for decryption
    - The decryption key cannot be derived from the encryption key!
    - Called “Public” because the encryption key can be made public and not compromise the security of the algorithm
    - Ex. RSA
  - What is a good algorithm? What is a bad algorithm?
- RSA (Rivest, Shamir and Adleman) 
  - Most commonly-used public key algorithm
  - You can read the original paper [here](http://people.csail.mit.edu/rivest/Rsapaper.pdf) (It’s a fun read! I promise!) 
  - Public Key Algorithm
  - Relies on the fact that it’s difficult to factor large numbers and the RSA problem
   - Both of which are considered mathematically hard problems

## Workshop Project Info (including workshop wiki, slides and examples)
https://github.com/annalorimer/htn-security-workshop

## Resources 
- Applied Cryptography By Bruce Schneier 
- Security in Computing By Charles P. Pfleeger; Shari Lawrence Pfleeger; Jonathan Margulies
- http://www.schneier.com/blog/
- O’Reilly Security Podcast
- Cryptography I by Dan Boneh (www.coursera.com)
- https://www.crypto101.io/
- https://en.wikipedia.org/wiki/Alice_and_Bob
- http://people.csail.mit.edu/rivest/Rsapaper.pdf
- Codebreakers By David Kahn
