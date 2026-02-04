# 📁 File Recovery & Data Validation using Python

## 🧠 Overview
This project applies analytical thinking and Python programming to solve a real-world data integrity problem — where files appear to be copied to external storage (like a pendrive) but are missing, corrupted, or unreadable.

Instead of simply relying on visible confirmation, this solution verifies file presence and ensures only valid files are recovered for further use.

---

## 🎯 Problem Statement
When files are copied manually:
- They may appear to copy successfully  
- The system shows no error  
- But the files are actually missing or corrupted  

This can lead to:
✔ Data loss  
✔ Incorrect analysis results  
✔ Wasted time and rework  

This project focuses on **validating files before using them for analysis or insights**.

---

## 🛠️ Solution Approach

### 🔍 Step 1: File Presence Check
Using file explorer search (e.g., `*ch`), confirm whether the copied files actually exist in the destination folder before running recovery logic.

---

### 🐍 Step 2: Python-Based Content Validation
1. Read files in **binary mode**
2. Detect actual file type based on **content**, not extension
3. Classify files into:
   - ✅ Recoverable (valid content)
   - ❌ Corrupted / Unrecoverable
4. Copy only valid files to a user-defined output folder

This ensures that only reliable data is recovered and usable for further analysis.

---

## 🧰 Technologies Used
- Python 3  
- `filetype` library  
- Jupyter Notebook (.ipynb)

---

## 📦 Repository Contents

