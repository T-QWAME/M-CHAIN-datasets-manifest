
# Project Overview: M-CHAIN Dataset Manifest

This repository supports the reproducibility requirements of the M‑CHAIN research project.  
It provides a manifest and documentation for the public datasets used in the evaluation of M‑CHAIN, a multi-chain smart contract fuzzing system.

The repository does not store the datasets themselves.  
All datasets remain at their official research sources, in accordance with licensing and distribution guidelines.


## Purpose of This Repository

1. Provide a clear, public pointer to all datasets used in M‑CHAIN experiments.  
2. Pin the exact commit hashes used for reproducibility.  
3. Document the role of each dataset in the evaluation pipeline.  
4. Provide lightweight scripts for fetching the datasets.  
5. Give examiners and researchers an easy way to reproduce the dataset setup.


## Datasets Used

### 1. SmartBugs Curated  
A labeled vulnerability benchmark used for accuracy and detection‑rate reporting.  
Official source: https://github.com/smartbugs/smartbugs-curated [1](https://github.com/smartbugs/smartbugs-curated)

### 2. SmartBugs Wild  
A large real‑world corpus of approximately 47,398 Solidity contracts collected from Etherscan.  
Used for scale and stress testing.  
Official source: https://github.com/smartbugs/smartbugs-wild [2](https://github.com/smartbugs/smartbugs-wild)

### 3. SWC Registry Test Cases  
Canonical per‑weakness samples used for regression testing.  
Official source: https://github.com/SmartContractSecurity/SWC-registry  
(Registry no longer actively maintained since 2020.) [3](https://github.com/SmartContractSecurity/SWC-registry)[4](https://swcregistry.io/)

### Dataset descriptions and sizes  
SmartBugs documentation provides high‑level descriptions of the datasets and lists expected sizes.  
Reference: https://github.com/smartbugs/smartbugs/blob/master/doc/datasets.md [5](https://github.com/smartbugs/smartbugs/blob/master/doc/datasets.md)


## Why These Datasets?

These datasets were selected because:

- SmartBugs Curated provides labeled vulnerabilities suitable for benchmarking precision.  
- SmartBugs Wild provides large real‑world coverage to evaluate scalability under realistic conditions.  
- SWC Registry provides canonical examples for regression and taxonomy alignment.

This combination offers a balanced evaluation capturing both controlled benchmarks and real-world performance.


## Reproducibility

A complete manifest (`manifest.csv`) lists:
- Dataset names  
- Source URLs  
- Pinned commit hashes  
- Dates  
- Usage notes  

Lightweight download scripts (`get_datasets.ps1` and optional shell equivalents) are provided for convenience.


## Folder Structure (Local, Suggested)
