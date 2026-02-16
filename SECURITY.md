
# Security Policy for the M‑CHAIN Dataset Manifest

This repository provides documentation, manifest files, and reproducibility support for the datasets used in the M‑CHAIN research project.  
The datasets themselves are fetched from their official public sources, including:

- SmartBugs Curated (labeled benchmark) [1](https://github.com/smartbugs/smartbugs-curated)  
- SmartBugs Wild (real-world corpus ~47k contracts) [2](https://github.com/smartbugs/smartbugs-wild)  
- SWC Registry test cases (canonical vulnerability examples) [3](https://github.com/SmartContractSecurity/SWC-registry)  

SmartBugs documentation provides details on dataset structure and usage.  
[5](https://github.com/smartbugs/smartbugs/blob/master/doc/datasets.md)

Because this repository does not contain executable smart‑contract code, only documentation and metadata, the security scope is limited and clearly defined below.

---

## 1. Reporting a Security Issue

If you believe you have found a security issue related to:

- Incorrect dataset source URLs  
- Incorrect commit hashes or version metadata  
- Broken reproducibility scripts  
- Documentation that could mislead users into unsafe practices  

Please open an **Issue** on this repository with a clear description.

If your concern is sensitive, email the maintainer directly using the GitHub profile contact email.

**Do not submit vulnerability information publicly without first contacting the maintainer.**

---

## 2. Out‑of‑Scope Security Issues

The following are **not** considered security issues for this repository:

### ❌ Vulnerabilities in SmartBugs Curated  
This dataset is maintained at its official repository:  
https://github.com/smartbugs/smartbugs-curated  
[1](https://github.com/smartbugs/smartbugs-curated)  

Any vulnerability in those contracts is intentional, as they serve as labeled benchmarks.

---

### ❌ Vulnerabilities in SmartBugs Wild  
This dataset contains real‑world contracts collected from Etherscan and may contain known or unknown vulnerabilities by design.  
Official source: https://github.com/smartbugs/smartbugs-wild  
[2](https://github.com/smartbugs/smartbugs-wild)  

These remain under the licensing and purpose defined by the original dataset authors.

---

### ❌ Vulnerabilities in SWC Registry test cases  
These Solidity files intentionally contain documented weaknesses.  
Official source: https://github.com/SmartContractSecurity/SWC-registry  
[3](https://github.com/SmartContractSecurity/SWC-registry)  

Also note: the SWC Registry is no longer actively maintained since 2020.  
[4](https://swcregistry.io/)

---

### ❌ Vulnerabilities in third‑party analysis tools  
This repository does not include analysis tools such as Mythril, Slither, or SmartBugs itself.  
Issues with tools should be reported on their respective repositories, per their documentation and licensing.

---

## 3. Responsible Use of Datasets

Users fetching datasets (Curated, Wild, SWC) are responsible for:

- Respecting the original dataset licenses (as documented by SmartBugs and SWC authors)  
- Avoiding redistribution of Solidity files outside permitted use  
- Following best practices when analysing real or vulnerable contracts  
- Ensuring any experiments are run in a sandboxed or private environment  

SmartBugs documentation states that dataset files retain their original licensing and must not be redistributed independently.  
[5](https://github.com/smartbugs/smartbugs/blob/master/doc/datasets.md)


## 4. Safe Usage Guidelines

For safe handling of datasets:

- Run analysis tools inside isolated environments (e.g., Docker, WSL, VM).  
- Avoid deploying dataset contracts onto public networks.  
- Handle vulnerable samples responsibly and only for academic or testing purposes.  
- Follow all guidelines from the original dataset authors.

## 5. Summary

This repository is a **metadata-only** reproducibility resource.  
It does not contain smart‑contract code and does not introduce direct security risks.  
Security issues should focus on the correctness and safety of the documentation, scripts, metadata, and reproducibility process.

If you have questions or concerns, please open an Issue or contact the maintainer directly.
