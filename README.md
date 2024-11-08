# **ASCON128 Encryption Algorithm**

Data security is crucial for maintaining the confidentiality of communications in digital systems. This project uses the **Ascon128** symmetric encryption algorithm to securely encrypt textual data. Developed in 2014 by cryptography experts Christoph Dobraunig, Maria Eichlseder, Florian Mendel, and Martin Schläffer, Ascon128 is based on a **permutation-substitution** architecture, using a **128-bit key** for optimal security.

Ascon128 is highly efficient, making it ideal for applications like secure communications, data storage, and IoT. Its lightweight, flexible design adapts easily to a wide range of platforms, including embedded systems and IoT devices, making Ascon128 a reliable choice for securing textual data in digital communications.

## Principle

The Ascon128 algorithm generates encrypted text and a **Tag** for verification when applied to plaintext and associated data. During decryption, the Tag, encrypted text, and associated data are used to retrieve the original plaintext. The algorithm performs **permutations** and **XOR operations** to achieve secure encryption.

## Structure

Ascon128 encryption follows a structured process to ensure secure data encryption:

1. **Three-Phase Permutation Process:**
   - **Addition of Round Constant**
   - **Substitution**
   - **Linear Diffusion**

2. **XOR Operations:**
   - Performed with specific variables to add further complexity and security.
   - The results are stored in registers, recording the final encrypted data and the Tag.

3. **Finite State Machine (FSM):**
   - Coordinates the encryption process, selecting and configuring control variables for each state, ensuring proper process management.

4. **Counters:**
   - Track the number of rounds and data blocks processed, ensuring synchronization of all algorithm modules within the FSM.

## How It Works

### Encryption Process
- The plaintext and associated data undergo a series of permutations.
- XOR operations add complexity to secure the data.
- The encrypted data and Tag are generated and stored.

### Decryption Process
- The algorithm uses the Tag, encrypted text, and associated data to retrieve the original plaintext.
