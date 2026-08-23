# 📊 Matplotlib & Seaborn

A practical **Data Visualization with Python** repository containing examples, Jupyter Notebooks, datasets, and projects using **Matplotlib, Seaborn, Pandas, and Plotly**.

This repository is designed for beginners and students who want to learn how to create meaningful charts, perform exploratory data analysis (EDA), and visualize real-world datasets using Python.

---

## 🚀 About the Project

Data visualization is an important part of **Data Science and Data Analytics**. It helps us understand patterns, trends, relationships, distributions, and comparisons in data.

This repository provides practical examples of:

* 📈 Basic plotting
* 📊 Statistical visualization
* 🔵 Distribution plots
* 📋 Categorical plots
* 🔥 Matrix/heatmap visualization
* 📉 Regression visualization
* 🏏 IPL data analysis
* 📊 Interactive visualization using Plotly
* 🔍 Exploratory Data Analysis (EDA)

---

## 🛠️ Technologies Used

* **Python**
* **Jupyter Notebook**
* **NumPy**
* **Pandas**
* **Matplotlib**
* **Seaborn**
* **Plotly**
* **Cufflinks**

---

## 📂 Repository Contents

| File                         | Description                                     |
| ---------------------------- | ----------------------------------------------- |
| `Matplotlib.ipynb`           | Basic and advanced plotting using Matplotlib    |
| `Categoricalplots.ipynb`     | Visualization of categorical data using Seaborn |
| `Distributionplot.ipynb`     | Distribution and statistical plots              |
| `Matrixplot.ipynb`           | Matrix-based visualizations such as heatmaps    |
| `Regression.ipynb`           | Regression plots and relationship analysis      |
| `Plotly_and_Cufflinks.ipynb` | Interactive data visualization                  |
| `Ipl_Capstone_Project.ipynb` | IPL dataset analysis and visualization          |
| `IPL.csv`                    | IPL dataset used for the capstone project       |
| `flights.csv`                | Flight-related dataset for visualization        |
| `tips.csv`                   | Restaurant tips dataset                         |
| `basicplot.png`              | Example visualization image                     |

The repository currently contains these notebooks and datasets.

---

# 📚 Topics Covered

## 1. Matplotlib

**Matplotlib** is a popular Python library used to create static, animated, and interactive visualizations.

### Important plots:

* Line Plot
* Bar Chart
* Histogram
* Scatter Plot
* Pie Chart
* Box Plot
* Area Plot
* Subplots
* Customization of charts

Example:

```python
import matplotlib.pyplot as plt

x = [1, 2, 3, 4, 5]
y = [10, 20, 15, 25, 30]

plt.plot(x, y)
plt.xlabel("X Values")
plt.ylabel("Y Values")
plt.title("Basic Line Plot")
plt.show()
```

---

## 2. Seaborn

**Seaborn** is a Python data visualization library built on top of Matplotlib. It provides attractive and informative statistical graphics.

### Important Seaborn plots:

* Scatter Plot
* Line Plot
* Bar Plot
* Count Plot
* Box Plot
* Violin Plot
* Histogram
* KDE Plot
* Pair Plot
* Heatmap
* Regression Plot

Example:

```python
import seaborn as sns
import matplotlib.pyplot as plt

data = sns.load_dataset("tips")

sns.scatterplot(
    data=data,
    x="total_bill",
    y="tip"
)

plt.show()
```

---

# 📊 Categorical Visualization

Categorical plots are used when data contains categories such as:

* Male / Female
* Product categories
* Departments
* Teams
* Cities
* Classes

Common plots include:

* Count Plot
* Bar Plot
* Box Plot
* Violin Plot

These plots help compare different categories and understand their distributions.

---

# 📈 Distribution Visualization

Distribution plots help us understand how numerical values are distributed.

Examples:

* Histogram
* KDE Plot
* Distribution Plot
* Box Plot

They can help identify:

* Central tendency
* Spread
* Skewness
* Outliers
* Data distribution

---

# 🔥 Matrix Visualization

Matrix plots are useful for visualizing relationships between multiple numerical variables.

One of the most commonly used matrix visualizations is a **Heatmap**.

Example:

```python
sns.heatmap(data.corr(), annot=True)
plt.show()
```

Heatmaps are especially useful for understanding **correlation between variables**.

---

# 📉 Regression Visualization

Regression plots help visualize the relationship between two variables.

For example:

```text
Study Hours  →  Exam Marks
```

A regression plot can help determine whether an increase in one variable is associated with an increase or decrease in another variable.

---

# 🏏 IPL Capstone Project

The repository also contains an **IPL Capstone Project** using `IPL.csv`.

The project demonstrates how visualization can be applied to a real-world sports dataset.

Possible analysis includes:

* Team performance
* Player performance
* Match statistics
* Runs
* Wickets
* Winning teams
* Season-wise analysis
* Data visualization

The main notebook is:

```text
Ipl_Capstone_Project.ipynb
```

---

# 📊 Datasets

The repository contains several datasets for practical visualization exercises.

### IPL Dataset

```text
IPL.csv
```

Used for IPL-related analysis and visualization.

### Flights Dataset

```text
flights.csv
```

Useful for studying trends in flight-related data.

### Tips Dataset

```text
tips.csv
```

A commonly used dataset for analyzing restaurant bills, tips, customers, and related variables.

---

# 🔍 Exploratory Data Analysis (EDA)

**Exploratory Data Analysis (EDA)** is the process of understanding a dataset before applying machine learning or statistical techniques.

A typical EDA workflow is:

```text
Dataset
   ↓
Data Cleaning
   ↓
Data Exploration
   ↓
Statistical Summary
   ↓
Data Visualization
   ↓
Pattern Detection
   ↓
Insights
```

Visualization plays an important role in identifying patterns and relationships within the data.

---

# 📌 Matplotlib vs Seaborn

| Feature            | Matplotlib                | Seaborn                           |
| ------------------ | ------------------------- | --------------------------------- |
| Type               | Visualization library     | Statistical visualization library |
| Built on           | Python plotting framework | Matplotlib                        |
| Customization      | Very high                 | High                              |
| Statistical plots  | Basic                     | Excellent                         |
| Ease of use        | Moderate                  | Easy                              |
| Default appearance | Basic                     | More attractive                   |
| Best for           | Detailed customization    | Statistical visualization         |

---

# ⚙️ Installation

Clone the repository:

```bash
git clone https://github.com/Monu-kumar-kushwaha/Matplotlib---Seaborn.git
```

Move into the project directory:

```bash
cd Matplotlib---Seaborn
```

Install the required libraries:

```bash
pip install numpy pandas matplotlib seaborn plotly cufflinks jupyter
```

Start Jupyter Notebook:

```bash
jupyter notebook
```

Open any `.ipynb` file and run the cells.

---

# 💻 Example Visualization Workflow

```python
import pandas as pd
import matplotlib.pyplot as plt
import seaborn as sns

# Load dataset
data = pd.read_csv("tips.csv")

# Display first five rows
print(data.head())

# Create visualization
sns.scatterplot(
    data=data,
    x="total_bill",
    y="tip"
)

plt.title("Total Bill vs Tip")
plt.show()
```

---

# 🎯 Learning Objectives

After completing this repository, you should be able to:

* Understand the basics of data visualization
* Create different types of charts
* Use Matplotlib effectively
* Use Seaborn for statistical visualization
* Visualize categorical data
* Analyze distributions
* Create correlation heatmaps
* Create regression plots
* Perform basic EDA
* Work with real-world datasets
* Build visualization-based projects

---

# 🌍 Real-World Applications

Data visualization is widely used in:

* 📊 Data Science
* 🤖 Machine Learning
* 💼 Business Analytics
* 💰 Finance
* 🏥 Healthcare
* 🛒 E-Commerce
* 🏏 Sports Analytics
* 📈 Marketing
* 🔬 Research
* 🎓 Education

### Example

A company can visualize monthly sales data to identify:

* Best-selling products
* Seasonal trends
* Revenue growth
* Low-performing products
* Customer behavior

---

# 🔮 Future Improvements

The repository can be expanded with:

* [ ] More real-world datasets
* [ ] Advanced EDA projects
* [ ] Interactive dashboards
* [ ] More Plotly examples
* [ ] Power BI integration
* [ ] Machine Learning visualization
* [ ] Time-series visualization
* [ ] Correlation analysis
* [ ] Advanced statistical plots
* [ ] More Data Science projects

---

# ⭐ Why This Repository?

This repository provides a **hands-on approach to learning Data Visualization with Python**.

Instead of learning visualization only through theory, you can practice with:

* Jupyter Notebooks
* Real datasets
* Statistical charts
* Data analysis
* Practical projects

It can be useful for **students, beginners, Data Science learners, and Python developers**.

---

# 👨‍💻 Author

**Monu Kumar Kushwaha**

GitHub:
https://github.com/Monu-kumar-kushwaha

---

# ⭐ Support

If you find this repository useful, consider giving it a ⭐ on GitHub.

Your support helps encourage further development and learning.

---

## 📄 License

This repository is created for **educational and learning purposes**.
