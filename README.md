# SAS_Biostats_Programming_Mani

## 📌 Purpose
This repository provides a **standardized SAS project structure** for biostatistical programming.  
It includes macros, SDTM/ADaM datasets, and TLFs (Tables, Listings, Figures), along with QC and logging setups.  
The goal is to make clinical trial programming **reproducible, organized, and compliant** with CDISC and regulatory expectations.

---

## 📂 Folder Structure

```text
SAS_Biostats_Programming_Mani/
├── macros/                  # Reusable SAS macros
├── python_scripts/          # Python helpers for QC, conversions, automation
├── autoexec.sas             # Auto-loads macros and libraries
├── data/                    # Data & outputs (⚠️ not stored in GitHub)
│   ├── raw/
│   ├── sdtm/
│   │   ├── logs/
│   │   ├── qc/
│   │   │   ├── compare/
│   │   │   └── logs/
│   │   ├── xpt/
│   │   └── specs/
│   ├── adam/
│   │   ├── logs/
│   │   ├── qc/
│   │   │   ├── compare/
│   │   │   └── logs/
│   │   ├── xpt/
│   │   └── specs/
│   ├── tables/
│   │   ├── logs/
│   │   └── qc/
│   │       ├── compare/
│   │       └── logs/
│   ├── listings/
│   │   ├── logs/
│   │   └── qc/
│   │       ├── compare/
│   │       └── logs/
│   └── figures/
│       ├── logs/
│       └── qc/
│           ├── compare/
│           └── logs/
│
├── programs/                # SAS programs
│   ├── sdtm/                # SDTM programs
│   ├── adam/                # ADaM programs
│   ├── tables/              # Table programs
│   ├── listings/            # Listing programs
│   ├── figures/             # Figure programs
│   └── qc/                  # QC programs
│       ├── sdtm/
│       ├── adam/
│       ├── tables/
│       ├── listings/
│       └── figures/
│
└── README.md

```
---

## 🚀 Usage

1. Clone the repository:  
   `git clone git@github.com:manivannan-mathiazhagan/SAS_Biostats_Programming_Mani.git`

2. Place raw datasets into the **data/raw/** folder (⚠️ do not push clinical data to GitHub).

3. Run **autoexec.sas** to set up libraries and macro paths.  
   - This links `data/` subfolders (SDTM, ADaM, TLFs) and QC folders.  
   - It also auto-loads macros from the `macros/` directory.

4. Develop programs in **programs/sdtm/**, **programs/adam/**, **programs/tables/**, **programs/listings/**, and **programs/figures/**.

5. Place QC programs in **programs/qc/** with subfolders for SDTM, ADaM, Tables, Listings, and Figures.  
   - Each QC data folder contains a `compare/` and `logs/` subfolder for validation and documentation.

---

## ⚠️ Data Handling

- **Do not commit actual data** (`.sas7bdat`, `.xpt`, `.csv`) to GitHub.  
- Use GitHub only for **programs, macros, specs, and scripts**.  
- Data should remain in secure company storage (e.g., P:/, Y:/, ODA server).  
- The repository provides placeholders (`data/`) to mimic project folder organization.

---

## 👤 Author
**Manivannan Mathialagan**  
Biostats Programming Enthusiast | SAS, Python, Automation
 📧 Email: [manivannan.mathiazhagan@gmail.com](mailto:manivannan.mathiazhagan@gmail.com) 
