# ZOC Tracker White Paper (Version 1.2.0)

The official White Paper for the ZOC (Zombie On Chain) methodology and the **Analytical Data Ingestion Platform (ADIP)** architecture.

**ZOC Tracker:** A specialized infrastructure for quantifying and tracking "Zombie On Chain" smart contracts. The user interface and brand identity are known as **Z-Terminal**.

The ZOC Tracker project introduces a new taxonomy and methodology to identify deployed smart contracts that are **functionally abandoned** or **economically negligible** on the blockchain.

### The ZOC Concept (Zombie On Chain)

The term ZOC is used to denote **persistent yet non-functional code** (Digital Debris). This phenomenon is a structural consequence of blockchain immutability, leading to the accumulation of "digital debris."

A contract is classified as a ZOC if it meets two quantifiable criteria:

* **Temporal Criterion (X):** A continuous external inactivity of at least **nine months** (initial working assumption).
* **Value Criterion (Y):** A **negligible total economic value** (Native Balance < 0.001 ETH and secondary assets < 10 USD – thresholds are adjustable).

### Advanced Methodology & Risk Quantification

To ensure high analytical precision, the ZOC methodology incorporates **advanced exclusion criteria** (introduced in V1.1.0) to differentiate genuine ZOCs from **strategically dormant contracts** (e.g., Multisigs awaiting quorum, unexpired Vesting contracts, or essential Proxy/Library contracts).

**V1.2.0 Key Update:** The system quantifies risk using the **ZOC Score (0-100)**, a metric that combines Danger, Impact, and Obsolescence for immediate prioritization of audit targets.

### ZOC Tracker Architecture and Objectives

The analytical tool aims to turn this diagnosis into an opportunity, built on the core **ADIP** architecture:

* **ADIP (Platform for Analytical Data Ingestion):** Infrastructure powered by **Go** (for concurrent ingestion) and **ClickHouse** (for massive analytical storage) to process the entire EVM history.
* **Chain Audit:** Provide an honest metric of network vitality by filtering out abandoned code.
* **Security & Education:** Identify dangerous contracts and locked contracts, creating the largest **Failure Data Repository** for audit tools.
* **Traffic Recovery:** Identify **Abandoned ZOCs** that still receive residual calls to redirect this traffic to healthy protocols.

### Contribution

We welcome community contributions on the following areas:

* Empirical validation of criteria (X and Y) and the **ZOC Score** model.
* Development of the indexing pipeline (see Section 3.1 of the White Paper).
* Implementation of ZOC classification models.

### Licensing

This repository uses a dual-licensing structure to distinguish between code and documentation.

**Documentation (ZOC White Paper):** The entirety of the White Paper is distributed under the **Creative Commons Attribution 4.0 International (CC BY 4.0)** license. You are free to use, share, and adapt this work, provided explicit credit is given to the ZOC Tracker methodology.

**ZOC Tracker Code (Future):** The source code for the ZOC Tracker tool, once published in this repository, will be distributed under the **MIT License**.

***

### Official Versions

Please check the [latest official Release (v1.2.0)](https://github.com/zoctracker/whitepaper-zoc/releases) for documentation and official artifacts.

* [White Paper ZOC (English)](https://github.com/zoctracker/whitepaper-zoc/blob/main/WHITEPAPER_ZOC_Eng.pdf)
* [White Paper ZOC (Français)](https://github.com/zoctracker/whitepaper-zoc/blob/main/WHITEPAPER_ZOC_Fr.pdf)
