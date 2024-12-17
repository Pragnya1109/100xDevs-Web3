# Cryptography

- Cryptography is a technique of securing information and communications through the use of codes so that only those persons for whom the information is intended can understand and process it.

- In Cryptography, the techniques that are used to protect information are obtained from mathematical concepts and a set of rule-based calculations known as algorithms to convert messages in ways that make it hard to decode them.

- These algorithms are used for cryptographic key generation, digital signing, and verification to protect data privacy, web browsing on the internet and to protect confidential transactions such as credit card and debit card transactions.

- Some terminologies related to Cryptography:

  - **Encryption**: Conversion of normal text to a random sequence of bits.
  - **Key**: Some amount of information is required to get the information of the cryptographic algorithm.
  - **Decryption**: The inverse process of encryption, conversion of a Random sequence of bits to plaintext.
  - **Cipher**: The mathematical function, i.e. a cryptographic algorithm which is used to convert plaintext to ciphertext(Random sequence of bits).

Today, encryption is an integral part of many of the tools and protocols we rely on to protect the security of our everyday transactions and online communications. Encryption can be used on the physical layer of the Internet to scramble data that’s being transmitted via cable or radio communications. It adds support for secure communications to plaintext protocols like the Hypertext Transfer Protocol (HTTP), which enables Web browsing, and can protect the integrity of data exchanged through applications like email and mobile messengers. You can also encrypt data that is stored on devices like cellphones or computers, shielding the local copies of emails, text messages, documents, and photos from unauthorized snooping.

How and at what layer your data is encrypted makes a huge difference. Just because a product or service uses encryption doesn’t necessarily mean that everything that’s stored on or sent over that platform is completely private. For example, Google now makes the HTTPS protocol (HTTP over an encrypted connection) the default for all Gmail traffic, which prevents unauthorized users from reading emails while they travel between Google’s email servers and end users’ computers — but it does nothing to stop Google itself from accessing plaintext copies of those conversations. If you don’t want your email provider to be able to read your messages, you have to take additional steps to implement end-to-end encryption, which refers to a system in which “messages are encrypted in a way that allows only the unique recipient of a message to decrypt it, and not anyone in between.” With end-to-end encryption, you encrypt the contents of a message on your local machine or device. That data is then transmitted as ciphertext by the email provider to the intended recipient, who is the only person who can decrypt and read it.

## Features Of Cryptography

1. **Confidentiality**: Information can only be accessed by the person for whom it is intended and no other person except him can access it.

2. **Integrity**: Information cannot be modified in storage or transition between sender and intended receiver without any addition to information being detected.

3. **Non-repudiation**: The creator/sender of information cannot deny his intention to send information at a later stage.

4. **Authentication**: The identities of the sender and receiver are confirmed. As well destination/origin of the information is confirmed.

5. **Interoperability**: Cryptography allows for secure communication between different systems and platforms.

6. **Adaptability**: Cryptography continuously evolves to stay ahead of security threats and technological advancements.

## How does cryptography work?

A cryptographic algorithm, or cipher, is a mathematical function used in the encryption and decryption process.

A cryptographic algorithm works in combination with a
key—a word, number, or phrase—to encrypt the plaintext. The same plaintext
encrypts to different ciphertext with different keys.

The security of encrypted data is
entirely dependent on two things: the strength of the cryptographic algorithm and the
secrecy of the key

---

# Types of Cryptography

### 1. Symmetric Key Cryptography

---

When the plaintext is encrypted and decrypted using the same key, it is know as symmetric encryption. It is also known as **_shared-key_** or **_private-key_** encrytption.

The only problem is that the sender and receiver exchange keys in a secure manner.

The most popular symmetric key cryptography systems are **_Data Encryption Systems (DES)_** and **_Advanced Encryption Systems (AES) ._**

### 2. Asymmetric Key Cryptography

---

This cryptographic method uses different keys for the encryption and decryption process.

Also known as **Public key cryptography**

This encryption method uses **_public_** and **_private key_** methods.

This public key method help completely unknown parties to share information between them like email id. private key helps to decrypt the messages and it also helps in the verification of the digital signature.

> The mathematical relation between the keys is that the private key cannot be derived from the public key, but the public key can be derived from the private key. Example: ECC,DSS etc.

The most widely used public-key cryptosystem is **_RSA (Rivest–Shamir–Adleman)_**. The difficulty of finding the prime factors of a composite number is the backbone of RSA.

### Weakness of the Public Key Encryption :

Public key Encryption is vulnerable to [Brute-force attack](https://www.cloudflare.com/learning/bots/brute-force-attack/).

This algorithm also fails when the user lost his private key, then the Public key Encryption becomes the most vulnerable algorithm.

Public Key Encryption also is weak towards [Man in the middle attack](https://www.wiz.io/academy/man-in-the-middle-attack). In this attack a third party can disrupt the public key communication and then modify the public keys.

If user private key used for certificate creation higher in the PKI (Public Key Infrastructure) server hierarchy is compromised, or accidentally disclosed, then a “man-in-the-middle attack” is also possible, making any subordinate certificate wholly insecure. This is also the weakness of public key Encryption.

### Applications of the Public Key Encryption :

1. **_Encryption/Decryption_**: Confidentiality can be achieved using Public Key Encryption. In this the Plain text is encrypted using receiver public key. This will ensure that no one other than receiver private key can decrypt the cipher text.

2. **_Digital signature_**: Digital signature is for senders authentication purpose. In this sender encrypt the plain text using his own private key. This step will make sure the authentication of the sender because receiver can decrypt the cipher text using senders public key only.

3. **_Key exchange_**: This algorithm can use in both Key-management and securely transmission of data.

   Public key cryptography is used by the **_Secure Sockets Layer (SSL)_** and **_Transport Layer Security (TLS)_** protocols to encrypt data sent between the web server and the client, establishing a secure channel for communication.

## Types of Cryptography Algorithm

- **Advanced Encryption Standard (AES)**: AES (Advanced Encryption Standard) is a popular encryption algorithm which uses the same key for encryption and decryption It is a symmetric block cipher algorithm with block size of 128 bits, 192 bits or 256 bits. AES algorithm is widely regarded as the replacement of DES (Data encryption standard) algorithm.

- **Data Encryption Standard (DES)**: DES (Data encryption standard) is an older encryption algorithm that is used to convert 64-bit plaintext data into 48-bit encrypted ciphertext. It uses symmetric keys (which means same key for encryption and decryption). It is kind of old by today’s standard but can be used as a basic building block for learning newer encryption algorithms.

- **RSA**: RSA is an basic asymmetric cryptographic algorithm which uses two different keys for encryption. The RSA algorithm works on a block cipher concept that converts plain text into cipher text and vice versa.

- **Secure Hash Algorithm (SHA)**: SHA is used to generate unique fixed-length digital fingerprints of input data known as hashes. SHA variations such as SHA-2 and SHA-3 are commonly used to ensure data integrity and authenticity. The tiniest change in input data drastically modifies the hash output, indicating a loss of integrity. Hashing is the process of storing key value pairs with the help of a hash function into a hash table.
