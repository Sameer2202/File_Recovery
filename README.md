# File Recovery & Data Validation using Python

## Overview
This project demonstrates how analytical thinking can be applied to solve a real-world data integrity problem, where files copied to external storage (such as a pendrive) appear successful but are missing or corrupted.

The solution verifies file presence at the system level and then applies Python-based content validation to recover only usable files.

---

## Problem Statement
In many cases:
- Files seem to be copied correctly
- No error message is shown
- But files are missing, unreadable, or corrupted

This can lead to data loss and incorrect analysis.  
This project focuses on verifying data existence and data quality before further use.

---

## Solution Approach
1. Verify whether files actually exist using wildcard search (for example, `*ch`) in the file explorer.
2. Read files in binary mode using Python.
3. Detect the actual file type based on file content, not file extension.
4. Separate recoverable files from corrupted ones.
5. Copy only valid files to a user-defined output location without modifying the original data.

---

## Technologies Used
- Python 3
- filetype library
- Jupyter Notebook / Google Colab

---

## Repository Contents
- `Files_Recover.ipynb` – Jupyter Notebook containing file recovery and validation logic  
- `README.md` – Project documentation  

---

## How to Run
1. Clone the repository.
2. Install the required dependency:
   ```bash
   pip install filetype
