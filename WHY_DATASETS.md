
# Why These Datasets Were Selected

This document explains the motivation for selecting the three public datasets used in the M‑CHAIN evaluation: **SmartBugs Curated**, **SmartBugs Wild**, and the **SWC Registry test cases**. These datasets provide coverage across labeled benchmarks, large real‑world corpora, and canonical vulnerability examples used throughout smart‑contract security research.


## 1. SmartBugs Curated (Labeled Benchmark)

**Source:** https://github.com/smartbugs/smartbugs-curated [1](https://github.com/smartbugs/smartbugs-curated)  
SmartBugs Curated is a widely referenced benchmark of **annotated vulnerable Solidity contracts**, each labeled with known vulnerability types. It is designed to support **detection‑rate evaluation**, making it ideal for validating:
- accuracy,
- true‑positive rate, and
- consistency across vulnerability types.

The repository includes tagged vulnerabilities following structured taxonomies documented in SmartBugs resources and related literature. Because the dataset is curated and manually annotated, it provides a controlled environment for evaluating detection quality objectively.

**Why M‑CHAIN uses SmartBugs Curated**
- Allows direct comparison of detection rates against baselines.  
- Provides clean, labeled ground truth for evaluation.  
- Recognized as a standard dataset in Ethereum security research.  

## 2. SmartBugs Wild (Large Real‑World Corpus)

**Source:** https://github.com/smartbugs/smartbugs-wild [2](https://github.com/smartbugs/smartbugs-wild)  
SmartBugs Wild is a corpus of **47,398 unique Solidity smart contracts** collected from Etherscan and processed into a research‑friendly format. Its documentation confirms the large scale and the methodology used to gather and preprocess these contracts.

This dataset is essential for evaluating:
- scalability,
- robustness,
- behavior on real‑world code, and
- performance under realistic workloads.

SmartBugs documentation includes size and metadata descriptions, allowing researchers to understand dataset composition. [3](https://github.com/smartbugs/smartbugs/blob/master/doc/datasets.md)

**Why M‑CHAIN uses SmartBugs Wild**
- Enables large‑scale benchmarking of throughput and coverage.  
- Provides contracts seen on mainnet, making evaluation realistic.  
- Helps measure performance on diverse, uncontrolled code samples.  


## 3. SWC Registry Test Cases (Auxiliary Regression Suite)

**Source:** https://github.com/SmartContractSecurity/SWC-registry [4](https://github.com/SmartContractSecurity/SWC-registry)  
The SWC Registry contains canonical examples of Solidity vulnerabilities, organized by **Smart Contract Weakness Classification (SWC)** categories. These examples serve as unit‑style checks across common Solidity weaknesses.

**Important note:**  
The SWC Registry is no longer actively maintained since 2020, and this is noted clearly in its documentation. Therefore, M‑CHAIN uses SWC only as an auxiliary regression set, not as a primary benchmark. [5](https://swcregistry.io/)

**Why M‑CHAIN uses SWC Registry**
- Useful for quick regression testing during development.  
- Provides simple, self‑contained vulnerability examples.  
- Aligns evaluation with standard SWC‑based taxonomies.  

## Why This Combination Is Strong

Using **Curated + Wild + SWC** gives M‑CHAIN coverage across three evaluation dimensions:

1. **Precision and recall** (Curated — labeled dataset)  
2. **Scalability and robustness** (Wild — large real‑world dataset)  
3. **Canonical behavior checks** (SWC — small regression set)

These datasets are documented across SmartBugs resources, which describe their sizes, structure, and intended usage in research. (https://github.com/smartbugs/smartbugs/blob/master/doc/datasets.md)

## Summary

| Dataset            | Role                                | Reason for Inclusion |
|--------------------|--------------------------------------|----------------------|
| SmartBugs Curated  | Labeled benchmark                    | Measures accuracy, TPR, and detection quality. |
| SmartBugs Wild     | Large real‑world corpus              | Tests scalability and real‑world robustness. |
| SWC Registry       | Auxiliary regression test cases      | Provides canonical examples; used for quick checks. |

This combination ensures a complete, academically sound evaluation and meets the reproducibility expectations for an MSc thesis.
