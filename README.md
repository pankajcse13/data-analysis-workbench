# 📊 Data Analyst Learning Project - Complete Guide for Freshers

> **Last Updated:** December 2024  
> **Author:** Nitish  
> **Status:** ✅ Ready to Learn!

---

## 🎯 What is a Data Analyst?

A Data Analyst collects, processes, and performs statistical analysis on data to help organizations make better decisions. They use tools like **Python**, **SQL**, **Excel**, and **visualization libraries** to extract insights from data.

---

## 🚀 Quick Start

```bash
# Step 1: Activate virtual environment
.venv\Scripts\activate

# Step 2: Install all required packages
pip install -r requirements.txt

# Step 3: Create practice database
python 00_Installation_Guide/05_Setup_Practice_Database.py

# Step 4: Start learning from 01_Python_Basics folder!
```

---

## 📁 Complete Project Structure

```
Data_analyis/
│
├── 📂 00_Installation_Guide/          # START HERE!
│   ├── 01_Python_Installation.md      # Python setup for Windows
│   ├── 02_SQL_Installation.md         # SQLite, MySQL, PostgreSQL guides
│   ├── 03_Study_Material_Syllabus.md  # 8-week learning roadmap
│   ├── 04_Python_Modules_List.py      # All packages reference
│   └── 05_Setup_Practice_Database.py  # Creates SQLite practice DB
│
├── 📂 01_Python_Basics/               # Week 1-2
│   ├── 01_variables_datatypes.py      # Variables, strings, numbers
│   ├── 02_data_structures.py          # Lists, Dictionaries, Tuples, Sets
│   ├── 03_functions_loops.py          # Functions, if-else, loops
│   └── 04_file_handling.py            # Read/Write CSV, JSON, TXT files
│
├── 📂 02_Python_Libraries/            # Week 3-4
│   ├── 01_numpy_tutorial.py           # NumPy for numerical computing
│   ├── 02_pandas_tutorial.py          # Pandas for data manipulation
│   └── 03_matplotlib_seaborn.py       # Data visualization
│
├── 📂 03_SQL_Learning/                # Week 5-6
│   ├── 01_basic_queries.sql           # SELECT, WHERE, ORDER BY
│   ├── 02_joins_and_unions.sql        # INNER, LEFT, RIGHT, FULL JOIN
│   ├── 03_aggregations.sql            # GROUP BY, COUNT, SUM, AVG
│   ├── 04_subqueries.sql              # Subqueries, CTEs, Window Functions
│   └── sample_database.sql            # Sample data for practice
│
├── 📂 04_Excel_Learning/              # Parallel Learning
│   ├── 01_excel_functions_guide.md    # VLOOKUP, IF, SUMIF formulas
│   ├── 02_pivot_table_guide.md        # Pivot tables & analysis
│   ├── 03_excel_visualization.md      # Charts & dashboards
│   ├── create_excel_files.py          # Script to generate Excel files
│   └── sample_data/                   # 6 Excel practice files
│       ├── sales_data.xlsx
│       ├── employee_data.xlsx
│       ├── product_inventory.xlsx
│       ├── customer_orders.xlsx
│       ├── financial_data.xlsx
│       └── survey_responses.xlsx
│
├── 📂 05_Projects/                    # Week 7-8
│   ├── project_1_sales_analysis.py    # Complete sales analysis project
│   └── project_2_customer_analysis.py # Customer segmentation project
│
├── 📂 06_Statistics/                  # Reference
│   └── statistics_basics.py           # Mean, Median, Mode, Std Dev
│
├── 📄 practice_database.db            # SQLite database (100+ records)
├── 📄 requirements.txt                # All Python packages
└── 📄 README.md                       # This file
```

---

## 🛠️ Tools & Installation

### ✅ Already Set Up
| Tool | Status | Location |
|------|--------|-----------|
| Python 3.13 | ✅ Installed | `.venv/` virtual environment |
| NumPy | ✅ Installed | Numerical computing |
| Pandas | ✅ Installed | Data manipulation |
| Matplotlib | ✅ Installed | Visualization |
| Seaborn | ✅ Installed | Statistical plots |
| OpenPyXL | ✅ Installed | Excel file handling |
| SQLite | ✅ Built-in | `practice_database.db` ready |

### 📥 Optional Tools to Install
| Tool | Purpose | Download |
|------|---------|----------|
| DB Browser for SQLite | Visual SQL editor | [sqlitebrowser.org](https://sqlitebrowser.org/) |
| MySQL | Production database | [dev.mysql.com](https://dev.mysql.com/downloads/) |
| Power BI | Dashboards | [powerbi.microsoft.com](https://powerbi.microsoft.com/) |
| Jupyter Notebook | Interactive coding | `pip install jupyter` |

---

## 📚 8-Week Learning Roadmap

| Week | Topic | Folder | Focus |
|------|-------|--------|-------|
| 1 | Python Basics | `01_Python_Basics/` | Variables, Data Types |
| 2 | Python Basics | `01_Python_Basics/` | Functions, Loops, Files |
| 3 | Python Libraries | `02_Python_Libraries/` | NumPy, Pandas basics |
| 4 | Python Libraries | `02_Python_Libraries/` | Pandas advanced, Matplotlib |
| 5 | SQL Fundamentals | `03_SQL_Learning/` | SELECT, WHERE, ORDER BY |
| 6 | SQL Advanced | `03_SQL_Learning/` | JOINs, GROUP BY, Subqueries |
| 7 | Projects | `05_Projects/` | Sales Analysis |
| 8 | Projects | `05_Projects/` | Customer Analysis |

> 📖 **Detailed syllabus:** See [03_Study_Material_Syllabus.md](00_Installation_Guide/03_Study_Material_Syllabus.md)

---

## 🚀 How to Run Files

### Python Files
```bash
# Activate virtual environment first
.venv\Scripts\activate

# Run any Python file
python 01_Python_Basics/01_variables_datatypes.py

# Or in VS Code: Open file → Press F5
```

### SQL Practice
```python
# In Python
import sqlite3
conn = sqlite3.connect('practice_database.db')
cursor = conn.cursor()
cursor.execute("SELECT * FROM employees")
print(cursor.fetchall())
```

### Excel Files
- Open files in `04_Excel_Learning/sample_data/` with Excel
- Follow guides in `04_Excel_Learning/` folder

---

## 💡 Key Skills & Resources

| Skill | Importance | Files to Study |
|-------|------------|----------------|
| Python | ⭐⭐⭐⭐⭐ | `01_Python_Basics/` |
| Pandas | ⭐⭐⭐⭐⭐ | `02_Python_Libraries/02_pandas_tutorial.py` |
| SQL | ⭐⭐⭐⭐⭐ | `03_SQL_Learning/` + `practice_database.db` |
| Excel | ⭐⭐⭐⭐ | `04_Excel_Learning/` + sample Excel files |
| Statistics | ⭐⭐⭐⭐ | `06_Statistics/statistics_basics.py` |
| Visualization | ⭐⭐⭐⭐ | `02_Python_Libraries/03_matplotlib_seaborn.py` |

---

## 📊 Practice Database

The `practice_database.db` contains:

| Table | Records | Description |
|-------|---------|-------------|
| departments | 6 | Company departments |
| employees | 20 | Employee details with salaries |
| customers | 12 | Customer information |
| products | 16 | Product catalog |
| orders | 15 | Order transactions |
| order_items | 28 | Order line items |

---

## 📧 Tips for Success

1. ⏰ **Practice daily** - 1-2 hours minimum
2. 🔍 **Google errors** - Stack Overflow is your friend
3. 📊 **Use real data** - Kaggle.com has free datasets
4. 💼 **Build projects** - Add to your portfolio
5. 📝 **Take notes** - Document what you learn

---

## 🎯 Next Steps After This Course

1. **Power BI / Tableau** - Data visualization tools
2. **Advanced SQL** - Window functions, optimization
3. **Machine Learning** - Scikit-learn basics
4. **Portfolio** - GitHub projects
5. **Certifications** - Google Data Analytics, IBM Data Science

---

**Happy Learning! 🚀**

*Created with ❤️ for aspiring Data Analysts*