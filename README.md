# SAS_Biostats_Programming_Mani

## 📌 Purpose
This repository provides a standardized SAS project structure for biostatistical programming, including macros, SDTM/ADaM datasets, and TLFs (Tables, Listings, Figures). It is intended as a reusable framework for clinical trial programming.

## 📂 Structure
- macros/ → Reusable SAS macros for datasets, QC, and outputs  
- python_scripts/ → Python helpers for QC, conversions, automation  
- sdtm/ → SAS programs for SDTM datasets  
- adam/ → SAS programs for ADaM datasets  
- tables/ → SAS programs for Tables  
- listings/ → SAS programs for Listings  
- figures/ → SAS programs for Figures  
- qc/ → QC programs, organized into SDTM, ADaM, Tables, Listings, Figures  
- data/ → Placeholders for raw/external data (not committed to GitHub)  
- autoexec.sas → Defines libraries and auto-loads macros  

## 🚀 Usage
1. Clone the repository using:  
   git clone git@github.com:manivannan-mathiazhagan/SAS_Biostats_Programming_Mani.git  

2. Place raw datasets into the data/ folder (⚠️ do not push to GitHub).  

3. Modify autoexec.sas to update library paths as needed.  

4. Run programs in sdtm/, adam/, tables/, listings/, and figures/.  

5. QC programs are available under the qc/ subfolders.  

## ⚠️ Data Handling
Raw and clinical trial data files should not be stored in GitHub due to size and confidentiality.  
Instead:  
- Keep only programs, macros, and specifications in GitHub.  
- Data should remain on your company’s secure storage (P:/, Y:/, or ODA server).  
- Programs will reference data through library paths defined in autoexec.sas.  

## 👤 Author
**Manivannan Mathialagan**  
Statistical Programming Manager  
