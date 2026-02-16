C:\mchain-data\README.md

# M-CHAIN Datasets Manifest

This directory contains pointers to all public datasets used to evaluate M-CHAIN.  
The datasets themselves remain at their official research sources to avoid license issues.

## Datasets and roles

- **SmartBugs Curated**  
  Labeled benchmark for detection-rate reporting.  
  Source: https://github.com/smartbugs/smartbugs-curated

- **SmartBugs Wild**  
  Large real-world corpus (~47k contracts).  
  Source: https://github.com/smartbugs/smartbugs-wild

- **SWC Registry test cases**  
  Auxiliary regression set (registry not actively maintained since 2020).  
  Source: https://github.com/SmartContractSecurity/SWC-registry

## How to fetch (Windows PowerShell)

```powershell
cd C:\mchain-data
git clone https://github.com/smartbugs/smartbugs-curated.git
git clone https://github.com/smartbugs/smartbugs-wild.git
git clone https://github.com/SmartContractSecurity/SWC-registry.git
