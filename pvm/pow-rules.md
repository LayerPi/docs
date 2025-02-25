---
description: POW Rules of pvm network
---

# POW Rules

### Overview 🌐

PVM’s Proof-of-Work (PoW) mechanism is designed to secure the network by rewarding miners for their computational contributions. In our system, miners compute SHA256 hashes to generate a random seed that meets a specific difficulty requirement. Valid proofs are submitted and tallied daily, ensuring fair and transparent distribution of PVM tokens.

***

### Mining Process ⛏️

1. **Hash Calculation:**\
   Miners compute a SHA256 hash based on a random seed. The goal is to produce a hash that meets our stringent difficulty requirement.
2. **Difficulty Requirement:**\
   A valid hash must **begin with the sequence `31415926`**. This specific prefix ensures that only computationally intensive and valid proofs-of-work are accepted.
3. **Submission of Valid Hash:**\
   Once a miner finds a valid hash, it is submitted to the network. Only hashes that start with `31415926` are considered valid and contribute to the daily tally.
4. **Continuous Mining:**\
   Miners continuously compute hashes throughout the day to maximize their chances of submitting valid proofs.

***

### Proof-of-Work (PoW) Algorithm Details 🔍

#### SHA256-Based Random Seed Generation

* **Algorithm:**\
  The SHA256 cryptographic hash function is used to compute a hash from a random seed.
*   **Target Difficulty:**\
    The hash must satisfy:

    ```
    hash.startswith("31415926")
    ```
