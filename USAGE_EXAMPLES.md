
# Usage Examples for M-CHAIN Dataset Environment

This file gives practical examples of how to use the datasets referenced in this repository.  
The examples help supervisors, examiners, and researchers verify dataset loading, dataset structure, and tool orchestration.

These examples rely on public dataset sources used in the M‑CHAIN thesis:
- SmartBugs Curated (labeled benchmark) [1](https://github.com/smartbugs/smartbugs-curated)  
- SmartBugs Wild (~47k real‑world Solidity contracts) [2](https://github.com/smartbugs/smartbugs-wild)  
- SWC Registry test cases (auxiliary regression set) [3](https://github.com/SmartContractSecurity/SWC-registry)  
- SmartBugs dataset documentation for dataset details and structure [5](https://github.com/smartbugs/smartbugs/blob/master/doc/datasets.md)  

---

## 1. Confirm Dataset Download Locations

Once datasets are cloned, verify folder locations:

### Windows PowerShell
```powershell
Get-ChildItem C:\mchain-data
