# Titanic Data Analysis With Data Visualization

## Project Overview
This project performs exploratory data analysis (EDA) and data visualization on the Titanic dataset using Python, Pandas, Matplotlib, and Seaborn.

The notebook demonstrates:
- Data loading and inspection
- Missing value handling
- Feature engineering
- Exploratory data analysis (EDA)
- Multiple visualization techniques
- Insight generation from passenger survival patterns

## Files Included

| File | Description |
|------|-------------|
| `Titanic_Data_Analysis_With_Data_Visualization.ipynb` | Main Jupyter notebook containing data cleaning, analysis, visualizations, and insights |
| `titanic_dataset.csv` | Titanic dataset used for the analysis |

---

## Dataset Information

The dataset contains passenger information including:

- PassengerId
- Survived
- Pclass
- Name
- Sex
- Age
- SibSp
- Parch
- Ticket
- Fare
- Cabin
- Embarked

Dataset size:
- 418 rows
- 12 columns

---

## Objectives

The project focuses on:

1. Cleaning the dataset.
2. Handling missing values.
3. Creating meaningful derived features.
4. Exploring survival patterns.
5. Building a mini visualization dashboard.
6. Extracting insights from visual analysis.

---

## Data Preparation

### Missing Value Handling

- Missing values in `Age` are filled using the median age.
- Missing values in `Fare` are filled using the median fare.
- The `Cabin` column is removed because it contains a large number of missing values.

### Feature Engineering

#### Age_Group
Passengers are categorized into age groups:

- Child (0–12)
- Teen (13–18)
- Young Adult (19–30)
- Adult (31–45)
- Middle-aged (46–60)
- Senior (61–80)

#### FamilySize
A new feature is created:

```python
FamilySize = SibSp + Parch
```

This represents the total family members traveling with a passenger.

---

## Visualizations

The notebook includes the following visualizations:

### 1. Age Distribution Histogram
Displays the distribution of passenger ages using a histogram with KDE.

**Purpose:** Understand age demographics of passengers.

### 2. Fare Distribution by Survival (Violin Plot)
Compares fare distributions between survivors and non-survivors.

**Purpose:** Examine the relationship between ticket fare and survival.

### 3. Survival Rate by Family Size (Bar Chart)
Shows how family size influences survival rate.

**Purpose:** Identify family-size trends in passenger survival.

### 4. Age Distribution by Passenger Class (Box Plot)
Compares age distributions across passenger classes.

**Purpose:** Analyze demographic differences between classes.

### 5. Survival Rate by Embarkation Port (Bar Chart)
Displays survival rates based on embarkation location.

**Purpose:** Investigate whether boarding location influenced survival.

### 6. Age vs Fare Scatter Plot
Plots passenger age against fare with survival information encoded visually.

**Purpose:** Explore relationships among age, fare, and survival.

### 7. Correlation Heatmap
Shows correlations among numerical features.

**Purpose:** Identify relationships between variables.

---

## Key Insights

- Passenger fare appears to be associated with survival probability.
- Survival rates vary across embarkation ports.
- Family size may influence survival outcomes.
- Passenger class exhibits demographic differences.
- Correlation analysis helps identify influential numerical variables.

---

## Installation

### Prerequisites

- Python 3.8+
- Jupyter Notebook

### Install Required Libraries

```bash
pip install pandas matplotlib seaborn notebook
```

---

## Usage

1. Clone or download the project files.
2. Ensure the dataset CSV is available.
3. Open the notebook:

```bash
jupyter notebook
```

4. Launch:

```text
Titanic_Data_Analysis_With_Data_Visualization.ipynb
```

5. Run all cells sequentially.

---

## Project Workflow

```text
Load Dataset
      ↓
Inspect Data
      ↓
Handle Missing Values
      ↓
Feature Engineering
      ↓
Exploratory Analysis
      ↓
Visualization Dashboard
      ↓
Insights & Conclusions
```

---

## Technologies Used

- Python
- Pandas
- Matplotlib
- Seaborn
- Jupyter Notebook

---

## Future Improvements

- Add interactive dashboards using Plotly.
- Perform statistical hypothesis testing.
- Build predictive machine learning models.
- Compare multiple classification algorithms.
- Create automated reporting.

---

## Author

Data Analysis and Visualization Project based on the Titanic dataset.

## License

This project is intended for educational and learning purposes.
