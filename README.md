# 📚 E-Library Data Insights

## 📌 Project Overview

**E-Library Data Insights** is a Python-based library management and data analysis project.

The project uses **Pandas, NumPy, Matplotlib, Seaborn, and Object-Oriented Programming (OOP)** concepts to load, clean, analyze, filter, and visualize library transaction data stored in a CSV file.

---

## ✨ Features

* 📂 Load library data from a CSV file
* ✅ Validate CSV file
* 🧹 Clean column names
* 📅 Convert dates into datetime format
* ⏱️ Calculate borrowing duration
* 🔄 Remove duplicate records
* 📋 Display library data
* 📊 Perform data analysis
* 👥 Find total transactions and users
* 📚 Find total books
* 🏆 Find Top 5 borrowed books
* 📖 Analyze genre distribution
* 📈 Calculate borrowing duration statistics
* 🔎 Filter by Genre
* ⏱️ Filter by Borrow Duration
* 📅 Filter by Borrow Date
* 📅 Filter by Return Date
* 📊 Generate Top 5 Books bar chart
* 📈 Generate Monthly Borrowing Trend line chart
* 🥧 Generate Genre Distribution pie chart
* 🔥 Generate Correlation Heatmap
* 🖥️ Menu-driven interface

---

## 🛠️ Technologies Used

| Technology | Purpose                                |
| ---------- | -------------------------------------- |
| Python     | Main programming language              |
| Pandas     | Data loading and data analysis         |
| NumPy      | Numerical and statistical calculations |
| Matplotlib | Data visualization                     |
| Seaborn    | Heatmap visualization                  |
| OOP        | Program structure                      |
| CSV        | Dataset format                         |

---

## 📦 Required Libraries

Install the required Python libraries using:

```bash
pip install pandas numpy matplotlib seaborn
```

---

## 📁 Project Structure

```text
E-Library-Data-Insights/
│
├── library_manager.py
├── library_transactions.csv
├── README.md
└── requirements.txt
```

> **Note:** Replace `library_manager.py` with your actual Python filename if it is different.

---

## 📊 Dataset Format

The CSV file should contain the following columns:

```text
Transaction_ID
User_ID
Book_Title
Genre
Borrow_Date
Return_Date
```

### Example

```csv
Transaction_ID,User_ID,Book_Title,Genre,Borrow_Date,Return_Date
T001,U001,Python Basics,Programming,2026-01-05,2026-01-15
T002,U002,Data Science,Programming,2026-01-10,2026-01-20
T003,U001,Atomic Habits,Self Help,2026-02-03,2026-02-13
```

The program automatically creates:

```text
Borrow_Duration
```

---

## 🚀 How to Run

### Step 1: Open the Project

Open the project folder in **VS Code**.

### Step 2: Install Libraries

Open the VS Code terminal and run:

```bash
pip install pandas numpy matplotlib seaborn
```

### Step 3: Run the Program

```bash
python library_manager.py
```

### Step 4: Enter CSV Filename

When the program asks:

```text
Enter CSV file name:
```

Enter:

```text
library_transactions.csv
```

Make sure the CSV file is located in the same folder as the Python file.

---

## 🖥️ Main Menu

```text
====================================
       E-LIBRARY MANAGEMENT
====================================

1. Show Data
2. Data Analysis
3. Filter Data
4. Top Books Chart
5. Borrowing Trend
6. Genre Chart
7. Correlation Heatmap
8. Exit
```

---

## 📋 Menu Options

### 1. Show Data

Displays the library transaction records.

### 2. Data Analysis

Displays:

* Total Transactions
* Total Users
* Total Books
* Top 5 Borrowed Books
* Genre Count
* Average Borrowing Duration
* Median Borrowing Duration
* Standard Deviation
* Minimum Borrowing Duration
* Maximum Borrowing Duration

### 3. Filter Data

Provides four filtering options:

1. Genre
2. Borrow Duration
3. Borrow Date
4. Return Date

### 4. Top Books Chart

Creates a **bar chart** showing the Top 5 Most Borrowed Books.

### 5. Borrowing Trend

Creates a **line chart** showing the monthly borrowing trend.

### 6. Genre Chart

Creates a **pie chart** showing borrowing distribution by genre.

### 7. Correlation Heatmap

Creates a **Seaborn heatmap** showing correlations between numerical columns.

### 8. Exit

Ends the program.

```text
Program ended successfully!
```

---

## 🧹 Data Cleaning

The program performs several data-cleaning operations.

### Remove Spaces from Column Names

```python
self.df.columns = self.df.columns.str.strip()
```

### Convert Dates

```python
pd.to_datetime(
    self.df[column],
    errors="coerce"
)
```

### Calculate Borrowing Duration

```python
self.df["Borrow_Duration"] = (
    self.df["Return_Date"]
    - self.df["Borrow_Date"]
).dt.days
```

### Remove Duplicate Records

```python
self.df.drop_duplicates(inplace=True)
```

---

## 🧠 Python Concepts Used

This project demonstrates:

* Classes and Objects
* Constructors
* Methods
* Conditional Statements
* `if`, `elif`, `else`
* `while` Loop
* User Input
* Exception Handling
* File Handling
* Pandas DataFrame
* NumPy
* Data Cleaning
* Data Filtering
* Data Analysis
* Data Visualization
* Object-Oriented Programming

---

## 📈 Visualizations

The project generates:

* 📊 Top 5 Books Bar Chart
* 📈 Monthly Borrowing Trend
* 🥧 Genre Distribution Pie Chart
* 🔥 Correlation Heatmap

---

## 🎯 Learning Outcomes

Through this project, you can practice:

* Working with real-world CSV datasets
* Data cleaning using Pandas
* Date and time handling
* Statistical analysis
* Data filtering
* Grouping and aggregation
* Data visualization
* Python OOP
* Building a menu-driven application

---

## 🔮 Future Improvements

Possible future improvements include:

* Add a graphical user interface (GUI)
* Add database support
* Add user authentication
* Add book availability tracking
* Add book issue/return functionality
* Add advanced analytics dashboard
* Export analysis reports
* Add more interactive visualizations

---
## ⭐ Project Status

**Completed – Python Data Analysis Project**
