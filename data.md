## Data Documentation
This document introduces and describes the exact data used by PTB-XL dataset.

### 1. Official Dataset

| Field | Value |
| :--- | :--- |
| Dataset | PTB-XL |
| Official dataset page | [PTB-XL ECG Dataset on PhysioNet](https://physionet.org/content/ptb-xl/) |
| Official repository | [physionet-ptb-xl on PhysioNet Code](https://physionet.org/content/ptb-xl/1.0.3/) |
| Paper | [PTB-XL, a large publicly available electrocardiography dataset](https://doi.org/10.1038/s41597-020-0495-6) |
| Dataset version | 1.0.3 |
| License | Creative Commons Attribution 4.0 International (CC BY 4.0) |
| Sampling Rates | 100 Hz / 500 Hz |
| Task | Binary Classification (Normal vs Abnormal) |

The complete official release contains:
- 21,799 12-lead ECG records from 18,885 patients, each lasting 10 seconds;
- `records100/` folder containing raw signal files (`.dat` and `.hea`) sampled at 100 Hz;
- `records500/` folder containing raw signal files (`.dat` and `.hea`) sampled at 500 Hz;
- `ptbxl_database.csv` containing clinical metadata, signal file paths (`filename_lr`, `filename_hr`), and predefined `strat_fold` assignments;
- `scp_statements.csv` mapping diagnostic codes (`scp_codes`) to standard diagnostic categories.

---

### 2. Data Used in This Project

The project utilizes all 21,799 records from the official release, loaded directly from the `records100/` directory (100 Hz sampling rate) and split strictly using the predefined `strat_fold` protocol (Folds 1–8 for Training, Fold 9 for Validation, Fold 10 for Testing) to prevent cross-patient data leakage.

| Item | Full official release | Used in this project |
| :--- | :--- | :--- |
| ECG Records | 21,799 | 21,799 |
| Source Folder | `records100/` & `records500/` | `records100/` |
| Sampling Rate | 100 Hz / 500 Hz | 100 Hz (1,000 time steps) |
| Signal Leads | 12 leads | 12 leads |
| Duration | 10 seconds | 10 seconds |
| Data Shape ($X$) | (21799, 1000, 12) | (21799, 1000, 12) |

The experimental subset class and split distribution:

| Class | Train (Folds 1–8) | Validation (Fold 9) | Test (Fold 10) | Total |
| :--- | :---: | :---: | :---: | :---: |
| Normal ($0$) | 7,263 | 918 | 918 | **9,099** |
| Abnormal ($1$) | 10,155 | 1,265 | 1,280 | **12,700** |
| **Total** | **17,418 (79.9%)** | **2,183 (10.0%)** | **2,198 (10.1%)** | **21,799 (100%)** |