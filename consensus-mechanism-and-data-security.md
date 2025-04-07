# Consensus Mechanism & Data Security

**Hybrid Consensus Mechanism (PoQ + DPoS)**

TixonEdge employs a hybrid consensus mechanism combining **Proof-of-Quality (PoQ)** and **Delegated Proof-of-Stake (DPoS)**.

* **PoQ (Proof-of-Quality)**: Node rewards are based not only on the amount of resources provided (e.g., data, computation) but also on the quality of task completion. For instance, when monitoring air quality, the accuracy and response time of the task completion will determine the node's weight in block production.
  * **Data-based Tasks**: For example, when multiple nodes monitor the same air quality parameters in a region, the consensus is achieved when a consistent result is verified and added to the blockchain.
  * **Computation-based Tasks**: Tasks are verified through deterministic tests (e.g., hash challenges) to ensure the authenticity of computational power.
* **DPoS (Delegated Proof-of-Stake) Governance Layer**: TixonEdge uses DPoS to elect super nodes, responsible for aggregating LightNode contribution proofs, cross-chain interactions, and reducing the main chain's load. Token holders vote to elect super nodes, ensuring decentralized governance.

**Privacy-Enhanced Data Marketplace**

TixonEdge ensures data privacy and security through the following mechanisms:

* **Device-level Trusted Execution Environment (TEE)**: Sensitive data is processed within the device's TEE and only output as de-identified features (e.g., "average daily energy consumption" instead of detailed usage patterns).
* **Data Ownership NFTization**: Each piece of data generates a unique NFT that records the device ID, timestamp, and hash value. NFTs enable data ownership traceability and allow buyers to purchase the data's usage rights via tokens. The original data contributors continue to receive a share of the revenue from subsequent data transfers.
* **Differential Privacy Injection**: Before being added to the blockchain, noise is injected into data to ensure individual data cannot be traced. For example, location data is obfuscated to a 1km radius to protect users' privacy.
