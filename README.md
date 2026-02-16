
# M-CHAIN Datasets Manifest

This repository lists the public datasets used in the evaluation of the **M‑CHAIN multi‑chain smart contract fuzzing system**.  
The datasets themselves are **not stored here** due to licensing and size constraints.  
Instead, this manifest provides **official download links**, **pinned commit hashes**, and **roles** for each dataset.

All sources referenced here are widely used in smart‑contract security research.

---

## 📁 Datasets and Roles

### 1. **SmartBugs Curated**  
- Purpose: Labeled benchmark used to evaluate detection rates and precision.  
- Source: https://github.com/smartbugs/smartbugs-curated  
- Notes: Contains annotated vulnerable Solidity contracts used for academic benchmarking.  
[1](https://github.com/smartbugs/smartbugs-curated)

---

### 2. **SmartBugs Wild**  
- Purpose: Large real‑world corpus (~47,000 Solidity contracts) used to evaluate scalability.  
- Source: https://github.com/smartbugs/smartbugs-wild  
- Notes: Extracted from Etherscan; widely used in research for large‑scale evaluation.  
[2](https://github.com/smartbugs/smartbugs-wild)

---

### 3. **SWC Registry Test Cases**  
- Purpose: Auxiliary regression tests for canonical vulnerability examples.  
- Source: https://github.com/SmartContractSecurity/SWC-registry  
- Notes: Registry is no longer actively maintained since 2020; used only for quick checks.  
[3](https://github.com/SmartContractSecurity/SWC-registry)[4](https://swcregistry.io/)

---

## 📄 Manifest File

This repository includes:

- `manifest.csv` — contains dataset names, descriptions, source URLs, pinned commit hashes, and metadata.

The commit hashes match the exact versions used in the thesis experiments.

---

## 📥 How to Fetch These Datasets (Windows PowerShell)

You may download the datasets directly into a local workspace using:

```powershell
cd C:\mchain-data
git clone https://github.com/smartbugs/smartbugs-curated.git
git clone https://github.com/smartbugs/smartbugs-wild.git
git clone https://github.com/SmartContractSecurity/SWC-registry.git
