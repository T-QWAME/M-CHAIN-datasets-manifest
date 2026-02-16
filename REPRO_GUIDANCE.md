
# Reproduction Guidance for M-CHAIN Dataset Setup

This document provides step-by-step guidance for reproducing the dataset environment used in the M‑CHAIN thesis.  
It relies on the public dataset sources and pinned commit hashes stored in this repository.

This guide covers:
1. Preparing the dataset workspace  
2. Fetching the datasets  
3. Verifying versions  
4. Running SmartBugs to confirm the dataset structure  
5. Ensuring full reproducibility  

---

## 1. Prepare the Dataset Workspace

Create a clean directory for the datasets:

### Windows PowerShell
```powershell
mkdir C:\mchain-data
cd C:\mchain-data
