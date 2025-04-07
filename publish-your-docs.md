# Technical Architecture

**Overall Architecture**

TixonEdge's architecture is based on a decentralized network model. Devices (including sensors, storage nodes, and computing nodes) automatically connect to the network through the LightNode architecture. Devices are dynamically assigned roles such as sensing, computing, or storage nodes based on hardware performance and network conditions. Blockchain technology ensures transparent resource scheduling, data ownership verification, and fair token-based rewards.

**LightNode**

* **Adaptive Protocol (LNAP)**: LightNodes use the adaptive protocol (LNAP) to dynamically adjust their network role. Devices do not require complex configuration and can easily participate in tasks. The power consumption and bandwidth requirements are minimal, with devices submitting lightweight proofs (such as zk-STARK) to the blockchain every 10 minutes or so, ensuring low energy consumption and high efficiency.
* **Dynamic Role Switching**: Devices automatically switch between roles based on their hardware performance and the task at hand. A device may act as a sensing node (collecting data), a computing node (providing edge computing power), or a storage node (caching and storing data). This flexibility improves the network's efficiency and scalability.
* **Anti-Ejection Mechanism**: To prevent resource overload and device ejection, TixonEdge supports containerized task isolation. This allows even older devices (e.g., Raspberry Pi 2) to participate in the network, contributing computing power and storage.

**DePIN Layer & Resource Pool**

The DePIN layer integrates globally distributed physical devices into a dynamic resource pool. These devices include various sensors (e.g., environmental sensors), edge computing devices (e.g., smartphones or edge computing boxes), and storage nodes. The DePIN layer allows TixonEdge to achieve global resource sharing across different devices, regions, and use cases.

**Blockchain Layer**

The blockchain layer records each device's resource contribution (e.g., sensor data, computational power, storage) in a decentralized ledger. When a device completes a task or contributes resources, the system automatically rewards the device with $SENSE tokens based on predefined rules. Smart contracts ensure the automation of resource allocation and task execution, eliminating the need for intermediaries and ensuring transparency, trust, and efficiency.
