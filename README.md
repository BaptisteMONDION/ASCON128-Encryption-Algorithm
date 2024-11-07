ASCON128 Encryption Algorithm

Data security is a key element in ensuring the confidentiality of communications in digital systems. In this project, we will use the symmetric encryption algorithm Ascon128 to effectively secure textual data. Developed in 2014 by cryptography experts Christoph Dobraunig, Maria Eichlseder, Florian Mendel, and Martin Schläffer, Ascon128 is based on a permutation-substitution architecture. It uses a 128-bit key to encrypt data, providing optimal security robustness.

Ascon128's high performance makes it an ideal choice for applications such as secure communications, data storage, and IoT devices. Additionally, its lightweight and flexible design allows it to easily adapt to a wide variety of platforms, including embedded systems and IoT devices. In summary, Ascon128 is an efficient and reliable symmetric encryption algorithm for securing textual data in digital communication systems.

Principle

When applied to plaintext and associated data, the ASCON algorithm generates encrypted text and a Tag used for verification. During the decryption process, the Tag, the encrypted text, and associated data are used to recover the original plaintext. The algorithm performs permutations and XOR operations during encryption.

Structure

The Ascon128 encryption algorithm follows a structured process to securely encrypt data. First, the data undergoes a three-phase permutation process, which includes:

- Addition of the round constant
- Substitution
- Linear diffusion
- 
Next, XOR operations are performed with specific variables to add an additional layer of complexity to the encryption. The resulting values are stored in registers to record the final encryption and the Tag value.

A Finite State Machine (FSM) is used to coordinate the encryption process by selecting and configuring control variables for each state. This ensures proper management of the process.

Finally, counters are employed to track the number of rounds and data blocks processed, ensuring consistency in the encryption process. These counters are essential for synchronizing the different modules of the algorithm within the FSM.

How it Works

Encryption Process:
The plaintext and associated data undergo a series of permutations.
XOR operations add complexity and security.
The encrypted data and Tag are generated and stored.

Decryption Process:
The algorithm uses the Tag, encrypted text, and associated data to recover the original plaintext.
