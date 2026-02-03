# 🐍 Python Installation Guide for Data Analysis

## Complete Step-by-Step Installation for Windows

---

## 📋 Table of Contents

1. [Download Python](#1-download-python)
2. [Install Python](#2-install-python)
3. [Verify Installation](#3-verify-installation)
4. [Install VS Code](#4-install-vs-code)
5. [Install Data Analysis Libraries](#5-install-data-analysis-libraries)
6. [Create Virtual Environment](#6-create-virtual-environment)
7. [Jupyter Notebook Setup](#7-jupyter-notebook-setup)
8. [Troubleshooting](#8-troubleshooting)

---

## 1. Download Python

### Step 1: Go to Python Official Website
```
https://www.python.org/downloads/
```

### Step 2: Download Latest Version
- Click the yellow button: **"Download Python 3.x.x"**
- The installer file will download (example: `python-3.12.0-amd64.exe`)

### Recommended Version
- **Python 3.10, 3.11, or 3.12** (Latest stable versions)
- Avoid Python 3.13+ for beginners (some libraries may not support yet)

---

## 2. Install Python

### Step 1: Run the Installer
- Double-click the downloaded `.exe` file

### Step 2: IMPORTANT - Check These Boxes ✅
```
┌─────────────────────────────────────────────────────────────┐
│  ☑ Add Python 3.x to PATH    ← VERY IMPORTANT!            │
│  ☑ Install launcher for all users (recommended)            │
└─────────────────────────────────────────────────────────────┘
```

### Step 3: Click "Install Now"
- Wait for installation to complete (2-5 minutes)
- Click "Close" when done

### Step 4: Restart Your Computer
- Restart to ensure PATH changes take effect

---

## 3. Verify Installation

### Open Command Prompt (cmd)
Press `Windows + R`, type `cmd`, press Enter

### Check Python Version
```cmd
python --version
```
**Expected Output:** `Python 3.12.0` (or your installed version)

### Check pip (Package Installer)
```cmd
pip --version
```
**Expected Output:** `pip 23.x.x from ...`

### Test Python
```cmd
python -c "print('Hello, Data Analyst!')"
```
**Expected Output:** `Hello, Data Analyst!`

---

## 4. Install VS Code

### Step 1: Download VS Code
```
https://code.visualstudio.com/download
```
- Click "Windows" button to download

### Step 2: Install VS Code
- Run the installer
- Check all options:
  - ☑ Add "Open with Code" action
  - ☑ Add to PATH
  - ☑ Register Code as editor

### Step 3: Install Python Extension
1. Open VS Code
2. Click Extensions icon (left sidebar) or press `Ctrl+Shift+X`
3. Search: **"Python"**
4. Install the one by Microsoft (first result)

### Step 4: Install Additional Extensions (Recommended)
- **Jupyter** - For notebooks
- **Python Indent** - Better indentation
- **autoDocstring** - Documentation helper
- **Pylance** - Better IntelliSense

---

## 5. Install Data Analysis Libraries

### Open Command Prompt or VS Code Terminal

### Install Core Libraries (One by One)
```cmd
pip install numpy
pip install pandas
pip install matplotlib
pip install seaborn
pip install openpyxl
pip install xlrd
```

### OR Install All at Once
```cmd
pip install numpy pandas matplotlib seaborn openpyxl xlrd scipy scikit-learn jupyter
```

### Library Purpose Table

| Library | Purpose | Example Use |
|---------|---------|-------------|
| **numpy** | Numerical computing | Arrays, math operations |
| **pandas** | Data manipulation | DataFrames, CSV/Excel reading |
| **matplotlib** | Basic plotting | Line charts, bar charts |
| **seaborn** | Statistical visualization | Heatmaps, distribution plots |
| **openpyxl** | Excel file handling | Read/write .xlsx files |
| **xlrd** | Legacy Excel support | Read old .xls files |
| **scipy** | Scientific computing | Statistics, optimization |
| **scikit-learn** | Machine learning | Prediction, clustering |
| **jupyter** | Interactive notebooks | Code + documentation |

### Verify Libraries Installed
```cmd
pip list
```

### Check Specific Library
```cmd
python -c "import pandas; print(pandas.__version__)"
```

---

## 6. Create Virtual Environment

### What is Virtual Environment?
A separate Python environment for each project to avoid conflicts.

### Create Virtual Environment
```cmd
# Navigate to your project folder
cd C:\Users\NITISH\Desktop\Data_analyis

# Create virtual environment
python -m venv .venv
```

### Activate Virtual Environment

**Windows Command Prompt:**
```cmd
.venv\Scripts\activate
```

**Windows PowerShell:**
```powershell
.venv\Scripts\Activate.ps1
```

**You'll see:** `(.venv)` at the beginning of your prompt

### Install Libraries in Virtual Environment
```cmd
pip install numpy pandas matplotlib seaborn openpyxl jupyter
```

### Deactivate When Done
```cmd
deactivate
```

---

## 7. Jupyter Notebook Setup

### Install Jupyter
```cmd
pip install jupyter notebook
```

### Start Jupyter Notebook
```cmd
jupyter notebook
```
- Browser will open automatically
- Navigate to your project folder
- Click "New" → "Python 3" to create notebook

### Jupyter Lab (Alternative - More Features)
```cmd
pip install jupyterlab
jupyter lab
```

### VS Code Jupyter (Recommended)
1. Install Jupyter extension in VS Code
2. Create file with `.ipynb` extension
3. Run cells directly in VS Code

---

## 8. Troubleshooting

### Problem: 'python' is not recognized
**Solution:**
1. Reinstall Python with "Add to PATH" checked
2. OR manually add to PATH:
   - Search "Environment Variables" in Windows
   - Edit PATH → Add `C:\Users\YourName\AppData\Local\Programs\Python\Python312\`

### Problem: pip not working
**Solution:**
```cmd
python -m pip install --upgrade pip
```

### Problem: Permission denied
**Solution:**
```cmd
pip install --user package_name
```

### Problem: SSL Certificate Error
**Solution:**
```cmd
pip install --trusted-host pypi.org --trusted-host files.pythonhosted.org package_name
```

### Problem: Module not found after installing
**Solution:**
- Make sure you're in the correct virtual environment
- Check: `pip show module_name`

---

## 📁 Recommended Project Structure

```
Data_analyis/
│
├── .venv/                    # Virtual environment
├── data/                     # Store your data files
│   ├── raw/                  # Original data
│   └── processed/            # Cleaned data
├── notebooks/                # Jupyter notebooks
├── scripts/                  # Python scripts
├── outputs/                  # Charts, reports
└── requirements.txt          # List of packages
```

### Create requirements.txt
```cmd
pip freeze > requirements.txt
```

### Install from requirements.txt
```cmd
pip install -r requirements.txt
```

---

## ✅ Quick Checklist

- [ ] Python installed (3.10+)
- [ ] Python added to PATH
- [ ] pip working
- [ ] VS Code installed
- [ ] Python extension installed
- [ ] Virtual environment created
- [ ] Core libraries installed (numpy, pandas, matplotlib, seaborn)
- [ ] Jupyter working

---

## 🎯 First Python Test

Create a file `test_setup.py`:

```python
# Test all installations
import numpy as np
import pandas as pd
import matplotlib.pyplot as plt
import seaborn as sns

print("✅ NumPy version:", np.__version__)
print("✅ Pandas version:", pd.__version__)
print("✅ Matplotlib version:", plt.matplotlib.__version__)
print("✅ Seaborn version:", sns.__version__)

# Quick test
data = pd.DataFrame({
    'Name': ['Alice', 'Bob', 'Charlie'],
    'Score': [85, 90, 78]
})
print("\n✅ Sample DataFrame:")
print(data)

print("\n🎉 All installations successful! You're ready to start learning!")
```

Run it:
```cmd
python test_setup.py
```

---

**Next:** Install SQL → See `02_SQL_Installation.md`