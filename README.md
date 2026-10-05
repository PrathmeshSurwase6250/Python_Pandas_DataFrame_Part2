# 🐼 Python Pandas DataFrame – Part 2

This repository contains my **intermediate-level Pandas practice** using Python and Jupyter Notebook.

The purpose of this repository is to strengthen my understanding of **Pandas DataFrames, data manipulation, filtering, sorting, grouping, handling missing values, applying functions, and performing practical data analysis**.

This is a continuation of my previous Pandas learning and focuses more on solving problems using real datasets and building data-analysis logic.

---

## 📚 Topics Covered

### 1. DataFrame Operations

- Creating and working with DataFrames
- Selecting rows and columns
- Accessing data using `loc` and `iloc`
- Adding and removing columns
- Updating column values
- Changing data types using `astype()`

```python
df["column"].astype("int")
```

---

### 2. Filtering Data

Practice with conditional filtering and multiple conditions.

```python
df[df["age"] > 25]

df[(df["age"] > 25) & (df["city"] == "Pune")]
```

Topics include:

- Single-condition filtering
- Multiple conditions
- `&` and `|`
- Boolean indexing
- Filtering specific columns

---

### 3. Sorting Data

Sorting DataFrames based on one or multiple columns.

```python
df.sort_values("salary", ascending=False)
```

Also practiced:

- Ascending sorting
- Descending sorting
- Multiple-column sorting
- Sorting after filtering

Example:

```python
df.sort_values(
    ["city", "salary"],
    ascending=[True, False]
)
```

---

### 4. Missing Values

Handling missing data using Pandas.

Topics include:

- Detecting missing values
- `isnull()`
- `notnull()`
- `dropna()`
- `fillna()`
- Forward fill
- Backward fill
- Filling missing values based on columns

Examples:

```python
df.isnull().sum()

df.dropna()

df.fillna(0)

df["column"].ffill()
```

---

### 5. Applying Functions

Using `apply()` to perform custom operations on Pandas columns.

Example:

```python
def check_player(players):
    return "V Kohli" in players

ipl["all_player"].apply(check_player)
```

This helps understand how custom Python functions can be applied to Pandas data.

---

### 6. `value_counts()`

Using `value_counts()` to calculate the frequency of values.

```python
df["city"].value_counts()
```

It is useful for:

- Counting categories
- Finding frequently occurring values
- Analysing categorical data
- Comparing values between columns

---

### 7. Grouping and Aggregation

Practicing grouped analysis using Pandas.

Important concepts include:

```python
df.groupby("city")
```

and aggregation functions such as:

- `sum()`
- `mean()`
- `min()`
- `max()`
- `count()`

Example:

```python
df.groupby("city")["sales"].sum()
```

---

### 8. Working with Real Datasets

This repository includes practical Pandas exercises using datasets such as:

- IPL data
- Movies data
- Student data
- Other structured datasets

The goal is to use Pandas on data that resembles real-world data-analysis problems rather than only working with small manually created DataFrames.

---

## 🏏 IPL Data Analysis

One of the major practice datasets is IPL data.

Examples of analysis include:

- Counting team appearances
- Finding match information
- Filtering matches by season
- Finding final matches
- Comparing teams
- Analysing players
- Working with player lists
- Finding team-wise statistics
- Creating custom functions for team analysis

Example:

```python
ipl["Team1"].value_counts() + ipl["Team2"].value_counts()
```

This type of analysis helps develop practical data manipulation and problem-solving skills.

---

## 🎬 Movies Data Analysis

The repository also includes practice with movie-related data.

Examples include:

- Working with missing movie titles
- Handling missing values
- Filtering movie records
- Working with columns containing links
- Using forward fill for missing values

Example:

```python
movies.dropna(subset=["title_x"])
```

and:

```python
movies["Link"].ffill()
```

---

## 🧠 Skills Practiced

Through this repository, I am developing practical knowledge of:

- Python
- Pandas
- DataFrames
- Data Cleaning
- Data Filtering
- Data Sorting
- Data Transformation
- Missing Value Handling
- Boolean Indexing
- Custom Functions
- `apply()`
- `value_counts()`
- `groupby()`
- Aggregation
- IPL Data Analysis
- Movie Data Analysis
- Jupyter Notebook

---

## 🛠️ Technologies Used

| Technology | Purpose |
|---|---|
| 🐍 Python | Programming language |
| 🐼 Pandas | Data manipulation and analysis |
| 📓 Jupyter Notebook | Practice and experimentation |
| 🔢 NumPy | Numerical operations |

---

## 🚀 Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/PrathmeshSurwase6250/Python_Pandas_DataFrame_Part2.git
```

### 2. Navigate to the project

```bash
cd Python_Pandas_DataFrame_Part2
```

### 3. Install Pandas

```bash
python3 -m pip install pandas
```

### 4. Install Jupyter Notebook

```bash
python3 -m pip install notebook
```

### 5. Start Jupyter Notebook

```bash
jupyter notebook
```

Then open:

```text
Middle.ipynb
```

---

## 📂 Repository Contents

```text
Python_Pandas_DataFrame_Part2/
│
└── Middle.ipynb
```

### `Middle.ipynb`

The main Jupyter Notebook containing my intermediate Pandas practice, examples, exercises, data manipulation, and analysis.

---

## 🎯 Learning Objective

The main objective of this repository is to move beyond basic Pandas syntax and develop the ability to **think in terms of data**.

Instead of only memorizing Pandas functions, I am practicing:

> **Understand the data → Ask a question → Write Pandas logic → Analyse the result**

This approach will help me prepare for the next stages of my **Data Science and Machine Learning journey**.

---

## 📈 Learning Progress

### Pandas Learning Path

- [x] Pandas Series
- [x] DataFrame Basics
- [x] DataFrame Indexing
- [x] Data Selection
- [x] Filtering
- [x] Sorting
- [x] Missing Values
- [x] `apply()`
- [x] `value_counts()`
- [x] GroupBy Basics
- [x] Real Dataset Practice
- [ ] Advanced GroupBy
- [ ] Merge & Join
- [ ] Pivot Tables
- [ ] Advanced Data Cleaning
- [ ] Pandas + Matplotlib
- [ ] Pandas + Seaborn
- [ ] End-to-End Data Analysis Projects

---

## 🔗 Repository

**GitHub:**  
https://github.com/PrathmeshSurwase6250/Python_Pandas_DataFrame_Part2

---

## 👨‍💻 Author

**Prathmesh Surwase**

Computer Engineering Student | Python | Pandas | Data Analysis | Machine Learning

---

⭐ If you find this repository useful, feel free to explore the notebooks and practice the examples yourself.

**Keep Learning. Keep Practicing. Keep Building. 🚀**
