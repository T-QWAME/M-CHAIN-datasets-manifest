
# Contributing to the M‑CHAIN Dataset Manifest

Thank you for your interest in contributing to the M‑CHAIN Dataset Manifest.  
This repository supports the reproducibility of the M‑CHAIN research project by providing:

- A dataset manifest (`manifest.csv`)
- Pinned commit hashes
- Download instructions
- Dataset rationale and documentation
- Lightweight setup scripts

This repository **does not** store any of the datasets themselves.  
Datasets remain at their official research sources:

- SmartBugs Curated (labeled benchmark) [1](https://github.com/smartbugs/smartbugs-curated)  
- SmartBugs Wild (~47k real‑world contracts) [2](https://github.com/smartbugs/smartbugs-wild)  
- SWC Registry test cases (auxiliary regression suite; not actively maintained since 2020) [3](https://github.com/SmartContractSecurity/SWC-registry)[4](https://swcregistry.io/)  

SmartBugs dataset documentation describes dataset usage, structure, and expected sizes.  
[5](https://github.com/smartbugs/smartbugs/blob/master/doc/datasets.md)

---

## 🧭 How You Can Contribute

### 1. Improve Documentation
You may update:

- PROJECT_OVERVIEW.md  
- WHY_DATASETS.md  
- DATASET_FAQ.md  
- REPRO_GUIDANCE.md  
- INSTALLATION.md  
- USAGE_EXAMPLES.md  

Documentation improvements are always welcome.

---

### 2. Propose Additional Guidance Files
You may suggest short, helpful files such as:

- Troubleshooting tips  
- IDE setup notes  
- Environment validation commands  

Any additions must remain lightweight and must **not** include dataset files.

---

### 3. Improve Scripts
You may enhance:

- `get_datasets.ps1` (Windows)  
- `get_datasets.sh` (Linux/macOS), if available  

Scripts should remain simple and only clone official dataset sources.

SmartBugs documentation uses Git-based dataset installation and therefore must remain the model for this repository.  
[6](https://github.com/smartbugs/smartbugs)

---

### 4. Report Issues
You may open an issue if:

- A dataset link changes  
- A commit hash needs updating  
- Instructions fail on a specific operating system  

Please include:
- OS version  
- Terminal/shell used  
- Exact error message  
- Steps to reproduce the issue  

---

## 🚫 What NOT to Contribute

To protect licensing, reproducibility, and repository integrity:

### ❌ Do NOT upload dataset files  
This includes files from:
- smartbugs‑curated repositories (Solidity files) [1](https://github.com/smartbugs/smartbugs-curated)  
- smartbugs‑wild repositories (47k+ contracts) [2](https://github.com/smartbugs/smartbugs-wild)  
- SWC Registry test cases (Solidity vulnerabilities) [3](https://github.com/SmartContractSecurity/SWC-registry)  

These datasets must remain at their official public sources.

---

### ❌ Do NOT upload large binaries or experimental results  
This repository is strictly metadata + documentation.

---

### ❌ Do NOT include Solidity contract code from external datasets  
SmartBugs documentation states that contract code retains the licensing of original repositories and must not be re‑distributed.  
[5](https://github.com/smartbugs/smartbugs/blob/master/doc/datasets.md)

---

## 📌 Contribution Workflow

1. Fork this repository.  
2. Create a new branch:  
   ```bash
   git checkout -b improve-docs
