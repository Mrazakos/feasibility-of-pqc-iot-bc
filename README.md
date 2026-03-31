# Project Repositories and Reproducibility

To ensure the total reproducibility of our research findings, we have open-sourced the source code, benchmarking suites, and reference implementations. The ecosystem is categorized into evaluation frameworks for performance metrics and a functional Proof of Concept (PoC) for the proposed protocol.

---

## Core Framework and Benchmarking

These repositories contain the tools and scripts used to generate the empirical data presented in the paper, focusing on cost efficiency, execution overhead, and latency.

* **[On-Chain Gas Profiling](https://github.com/Mrazakos/bc-crypto-storage)**
    * **Description:** This repository provides the environment for measuring the gas-cost on the Ethereum Virtual Machine (EVM).
    * **Key Components:** Includes Hardhat-based smart contracts and automated gas evaluation scripts.

* **[Off-Chain Edge Emulation](https://github.com/Mrazakos/vc-ecdsa-crypto)**
    * **Description:** This suite focuses on the performance of the protocol at the network edge, specifically targeting mobile and IoT environments where computational resources are limited.
    * **Key Components:** Features a custom W3C-compliant credentialing suite, mobile issuer performance metrics, and containerized IoT benchmarking scripts to simulate deployment on resource-constrained hardware.

## Proof of Concept (Reference Architecture)

The following repositories provide a complete, end-to-end implementation of the reference architecture. These components demonstrate the practical application of the protocol across the blockchain, mobile, and hardware layers.

| Component | Repository Link | Technical Role |
| :--- | :--- | :--- |
| **Mobile Application** | [access-control-app](https://github.com/Mrazakos/access-control-app) | Manages Decentralized Identifiers (DIDs), handles secure credential storage, and facilitates user-side request signing. |
| **Smart Lock** | [access-control-lock](https://github.com/Mrazakos/access-control-lock) | Simulates an IoT device that validates credentials and triggers hardware actions. |
| **Smart Contract** | [access-control-contract](https://github.com/Mrazakos/acces-control-contract) | Functions as the decentralized authority, managing authorization logic, credential revocation lists, and state transitions. |

---

> **Academic Note:** These resources are maintained to support peer review and future research in blockchain-based access control and Verifiable Credentials (VCs). Detailed setup instructions, dependency requirements, and configuration parameters are available in the documentation of each individual repository.
