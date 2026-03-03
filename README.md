# Iris Dataset Exploration - Task 1

# Task-1-Exploring_and_Visualizing_the_Dataset
## 📊 Project Overview
This project focuses on exploring and visualizing the famous Iris dataset as part of my internship task. The objective was to learn how to load, inspect, and visualize datasets to understand data trends and distributions.

## 🎯 Task Objectives
- Load dataset using pandas
- Inspect data structure and properties
- Generate summary statistics
- Create visualizations to understand relationships and patterns
- Identify outliers and distributions

## 📁 Dataset Information
The Iris dataset contains measurements of 150 iris flowers from three different species:
- **Setosa** (50 samples)
- **Versicolor** (50 samples)  
- **Virginica** (50 samples)

### Features:
- `sepal_length` (cm)
- `sepal_width` (cm)  
- `petal_length` (cm)
- `petal_width` (cm)
- `species` (target variable)

## 🛠️ Technologies Used
- **Python 3.10.11**
- **Pandas** - Data manipulation and analysis
- **Matplotlib** - Data visualization
- **Seaborn** - Statistical data visualization
- **Jupyter Notebook** - Interactive development

## 📈 Key Analyses Performed

### 1. Data Loading and Inspection
```python
# Load dataset
df = pd.read_csv("iris.csv")

# Basic information
print(df.shape)  # (150, 5)
print(df.columns)
df.info()
df.describe()
```

### 2. Data Quality Check
- ✅ No missing values found in any column
- ✅ All features are numerical (float64)
- ✅ Target variable is categorical (object)

### 3. Visualizations Created

#### Scatter Plots
- **Sepal Length vs Sepal Width** (basic and species-colored)
- **Petal Length vs Petal Width by Species** - Shows clear species separation

#### Distribution Analysis
- Histogram with KDE for petal length distribution
- Frequency distribution of sepal length

#### Outlier Detection
- Box plots for individual features
- Combined boxplot for all numerical features

## 🔍 Key Findings

1. **Species Separation**
   - Setosa is clearly distinguishable from other species
   - Petal features show better separation than sepal features

2. **Data Distribution**
   - All features are normally distributed with slight variations
   - No extreme outliers detected, though some minor outliers in sepal_width

3. **Feature Relationships**
   - Strong correlation between petal length and petal width
   - Setosa has significantly smaller petal measurements

## 📊 Sample Visualizations

The notebook includes:
- Species-wise scatter plots
- Distribution histograms
- Box plots for outlier detection
- Correlation patterns between features

## 🚀 How to Run

1. Clone this repository
2. Install required libraries:
   ```bash
   pip install pandas matplotlib seaborn jupyter
   ```
3. Open the Jupyter notebook:
   ```bash
   jupyter notebook "task-1-Exploring_and_Visualizing_the_Dataset.ipynb"
   ```
4. Run all cells to see the analysis

## 📁 Repository Structure
```
├── task-1-Exploring_and_Visualizing_the_Dataset.ipynb  # Main notebook
├── iris.csv                                            # Dataset
├── line_plot.png                                        # Saved visualization
└── README.md                                           # Project documentation
```

## ✅ Task Completion Checklist
- [x] Load dataset using pandas
- [x] Print shape and column names
- [x] Display first few rows with `.head()`
- [x] Use `.info()` and `.describe()` for statistics
- [x] Create scatter plots for relationship analysis
- [x] Generate histograms for distribution analysis
- [x] Create box plots for outlier detection
- [x] Utilize both matplotlib and seaborn libraries
- [x] Save visualizations as PNG files

## 📝 Conclusion
This exploration successfully demonstrates basic data analysis and visualization techniques using Python. The Iris dataset serves as an excellent example for understanding data patterns, species classification, and feature relationships.

---

---
**Submitted by**: DeveloperHC Intern
**Date**: March 4, 2026
**Internship Task**: Task 1 - Exploring and Visualizing a Simple Dataset
---
