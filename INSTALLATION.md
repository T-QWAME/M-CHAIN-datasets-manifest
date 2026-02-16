
and Setup Guide for M‑CHAIN Dataset Environment

This guide explains how to prepare the environment needed to download and manage the datasets used in the M‑CHAIN evaluation.  
The datasets themselves remain at their official public sources and are fetched via Git.

The instructions below cover:
1. Installing Git (Windows, macOS, Linux)  
2. Preparing the dataset workspace  
3. Fetching the datasets from their public sources  
4. Optional: Installing SmartBugs for dataset-aware tooling  

---

## 1. Install Git

The datasets are hosted on GitHub (SmartBugs Curated, SmartBugs Wild, SWC Registry), so Git is required to clone them.  
SmartBugs documentation and dataset repositories indicate Git cloning as the primary method of dataset retrieval.  
[4](https://github.com/smartbugs/smartbugs/blob/master/doc/datasets.md)[5](https://github.com/smartbugs/smartbugs)

### Windows
1. Download Git for Windows:  
   https://git-scm.com/download/win  
2. Run the installer.  
3. Accept default settings.  
4. After installation, verify in PowerShell:  
   ```powershell
   git --version
