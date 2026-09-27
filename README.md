# Digital Forensic Investigation Report  
**Case ID:** AIT-DF-2026-009  

**Organization:** Apex Integrated Technologies Ltd.  
**Investigation Title:** Digital Forensic Investigation – Deleted File Recovery  
**Investigator:** Chikere James  
**Date:** September 2026  

---

## Overview

This repository contains the final report and supporting documentation for a digital forensic examination conducted on a supplied forensic disk image (`Evidence.E01`).

The investigation focused on determining the status of six target folders that were reported missing from a workstation:

- SSH  
- My pic  
- Our pic  
- ADDS Project  
- Corel  
- Corel Draw Work  

The examination aimed to establish whether the folders were present, deleted, recoverable, or unrecoverable, and to determine the most defensible timeframe of relevant activity supported by the evidence.

---

## Key Findings

- Three of the six target folders (**SSH**, **Corel**, and **Corel Draw Work**) were identified as deleted directory entries and were recoverable.
- The remaining three folders (**My pic**, **Our pic**, and **ADDS Project**) could not be located or recovered.
- The filesystem was identified as **NTFS**.
- A working copy of the evidence was created and integrity was verified using SHA-256 and MD5.
- No evidence was found that attributes the deletion to a specific individual or establishes intent.

Full details, methodology, limitations, and supporting tables are contained in the report.

---

## Repository Structure
AIT-DF-2026-009_Digital_Forensics/
├── README.md
├── REPORT/
│   └── AIT-DF-2026-009_Final_Report.pdf          # Main forensic report
├── EVIDENCE/
│   ├── recovered/                               # Exported recovered files (sample)
│   └── hashes/
│       └── recovered_files_hashes.txt           # SHA-256 hashes of selected recovered files
├── LOGS/
│   ├── investigation_log.md
│   └── chain_of_custody.md
└── SCREENSHOTS/                                 # Supporting screenshots referenced in the report

---

## Important Notes

- The **original forensic image** (`Evidence.E01`) is **not** included in this repository for legal and privacy reasons.
- Only a representative sample of recovered files was hashed and documented due to the large number of items (particularly in the Corel Draw Work folder).
- All examination was performed on a verified working copy of the evidence.

---

## Tools Used

- DD  
- FTK Imager  
- Autopsy  
- R-Drive Image  

---

## Disclaimer

This investigation was conducted for academic/training purposes as part of a digital forensics assignment. The findings are based solely on the supplied forensic image and the tools specified in the assignment brief.
