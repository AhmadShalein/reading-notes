# Read 18: Cryptography:

## Encryption, Decryption & Hacking:

* **Cryptography** requires two steps: **encryption** and **decryption**. The encryption process uses a cipher in order to encrypt plaintext and turn it into ciphertext. Decryption, on the other hand, applies that same cipher to turn the ciphertext back into plaintext.

* **Encryption**: scrambling the data according to a secret key (in this case, the alphabet shift).

* **Decryption**: recovering the original data from scrambled data by using the secret key.

* **Code cracking**: uncovering the original data without knowing the secret, by using a variety of clever techniques.

* **Types of Cryptography**:

  * **Hashing**: Hashing is a type of cryptography that changes a message into an unreadable string of text for the purpose of verifying the message’s contents, not hiding the message itself.

  * **Symmetric Cryptography**: This type of cryptography uses a single key to encrypt a message and then decrypt that message upon delivery.

  * **Asymmetric Cryptography**: Asymmetric cryptography (as the name suggests) uses two different keys for encryption and decryption, as opposed to the single key used in symmetric cryptography. The first key is a public key used to encrypt a message, and the second is a private key which is used to decrypt them.

  * **Key Exchange Algorithms**.

----------------------------

## Ceasar Cipher:

* In cryptography, a **Caesar cipher**, also known as **Caesar’s cipher**, the **shift cipher**, **Caesar’s code** or **Caesar shift**, is one of the simplest and most widely known encryption techniques. It is a type of substitution cipher in which each letter in the plaintext is replaced by a letter some fixed number of positions down the alphabet.

* The **Caesar cipher** can be easily broken even in a ciphertext-only scenario. Two situations can be considered:

  * an attacker knows (or guesses) that some sort of simple substitution cipher has been used, but not specifically that it is a Caesar scheme.

  * an attacker knows that a Caesar cipher is in use, but does not know the shift value.

![Ceasar Cipher](https://upload.wikimedia.org/wikipedia/commons/thumb/4/4a/Caesar_cipher_left_shift_of_3.svg/1200px-Caesar_cipher_left_shift_of_3.svg.png)
