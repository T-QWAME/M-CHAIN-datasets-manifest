
# Glossary of Terms for the M‑CHAIN Dataset Manifest

This glossary defines key terms used throughout the M‑CHAIN dataset manifest, reproducibility package, and thesis documentation.  
It helps supervisors, examiners, and researchers understand the components of the dataset environment without needing prior knowledge of SmartBugs, SWC Registry, or Ethereum tooling.

---

## A

### **Annotation**
A short label or tag describing a known vulnerability in a contract.  
SmartBugs Curated uses annotated Solidity files to mark vulnerability locations.  
[1](https://github.com/smartbugs/smartbugs-curated)

---

## C

### **Commit Hash**
A unique Git identifier pointing to a specific version of a dataset or repository.  
This ensures strict reproducibility for SmartBugs Curated, SmartBugs Wild, and SWC Registry datasets.

### **Contract Dataset**
A collection of Solidity contracts used as benchmarks or evaluation sets.  
SmartBugs Curated and SmartBugs Wild are examples of contract datasets widely used in smart‑contract security research.  
[1](https://github.com/smartbugs/smartbugs-curated)[2](https://github.com/smartbugs/smartbugs-wild)

### **Curated Dataset**
A dataset that is intentionally selected and labeled for controlled evaluation.  
In this project, *SmartBugs Curated* serves as the curated, vulnerability‑annotated dataset.  
[1](https://github.com/smartbugs/smartbugs-curated)

---

## D

### **Dataset Manifest**
The `manifest.csv` file listing:
- dataset names  
- official source URLs  
- commit hashes  
- download dates  
- dataset roles  

This file makes the dataset setup replicable.

### **Documentation Set**
The collection of Markdown files (e.g., README, Installation, FAQ, etc.) that form the reproducibility platform.

---

## E

### **EVM (Ethereum Virtual Machine)**
The execution environment for Ethereum smart contracts.  
Many contracts in SmartBugs Wild are EVM‑compatible.  
[2](https://github.com/smartbugs/smartbugs-wild)

---

## F

### **Framework (SmartBugs Framework)**
A tool that orchestrates multiple analysis tools, manages compiler versions, and outputs normalized SARIF results.  
SmartBugs documentation explains how datasets are managed and how tools are invoked.  
[6](https://github.com/smartbugs/smartbugs)

---

## G

### **Git Clone**
The method used to download SmartBugs Curated, SmartBugs Wild, and SWC Registry.  
All referenced datasets are retrieved via public Git repositories.  
[1](https://github.com/smartbugs/smartbugs-curated)[2](https://github.com/smartbugs/smartbugs-wild)[3](https://github.com/SmartContractSecurity/SWC-registry)

---

## L

### **Labeled Dataset**
A dataset that includes explicit vulnerability annotations.  
SmartBugs Curated is labeled with multiple vulnerability categories and tags.  
[1](https://github.com/smartbugs/smartbugs-curated)

---

## M

### **Metadata**
Information about the dataset, including:
- commit hash  
- size of the dataset folder  
- download date  
- role in evaluation  

SmartBugs documentation lists metadata for Curated, Wild, and related datasets.  
[5](https://github.com/smartbugs/smartbugs/blob/master/doc/datasets.md)

---

## P

### **Pinned Version**
A fixed commit hash that ensures the exact dataset version used in the thesis can be downloaded again in the future.  
All datasets in this manifest use pinned versions.

---

## R

### **Regression Tests**
Small, deterministic tests run to ensure correctness.  
SWC Registry test cases are used for regression testing in smart‑contract analysis.  
[3](https://github.com/SmartContractSecurity/SWC-registry)[4](https://swcregistry.io/)

### **Reproducibility**
The ability to rebuild the same dataset environment using:
- pinned versions  
- verified download commands  
- consistent directory structure  
- manifest files  
- documented scripts  

SmartBugs documentation emphasizes this through dataset and framework consistency.  
[5](https://github.com/smartbugs/smartbugs/blob/master/doc/datasets.md)[6](https://github.com/smartbugs/smartbugs)

---

## S

### **SARIF**
A standardized output format for static analysis results.  
SmartBugs can aggregate vulnerability reports into SARIF format for consistency.  
[6](https://github.com/smartbugs/smartbugs)

### **SmartBugs Curated**
A labeled dataset containing annotated vulnerabilities for benchmarking precision and recall.  
[1](https://github.com/smartbugs/smartbugs-curated)

### **SmartBugs Wild**
A dataset of ~47,398 real‑world contracts gathered from Etherscan and structured for large‑scale testing.  
[2](https://github.com/smartbugs/smartbugs-wild)

### **SWC Registry**
A repository of canonical vulnerability test cases categorized by Smart Contract Weakness Classification (SWC).  
Public and static since 2020.  
[3](https://github.com/SmartContractSecurity/SWC-registry)[4](https://swcregistry.io/)

---

## T

### **Test Case**
A small, self‑contained contract illustrating a specific vulnerability.  
The SWC Registry consists of test cases for regression-style evaluation.  
[3](https://github.com/SmartContractSecurity/SWC-registry)

---

## U

### **Usage Examples**
Instructions showing how to:
- verify dataset folders  
- list SmartBugs datasets  
- run simple evaluations  
- explore dataset structure  

These examples support reproducibility and appear in `USAGE_EXAMPLES.md`.

---

## W

### **Wild Dataset**
A term used for SmartBugs Wild — referring to its uncontrolled, real‑world origin.  
It contains contracts collected from the Ethereum mainnet and is used for scalability evaluation.  
[2](https://github.com/smartbugs/smartbugs-wild)

---

## Z

### **Zero‑Configuration Fetch**
A setup where datasets can be fetched automatically using a script such as `get_datasets.ps1`, requiring no manual configuration beyond installing Git.

---
