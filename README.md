# Experiment 4: Data Wrangling and Data Visualization


## I. Intended Learning Outcomes
At the end of this laboratory activity, the student is able to:
1. Filter tabular data using several categorical and numerical conditions
3. Construct focused DataFrames by selecting relevant features
4. Summarize the relationship between categorical features and a numerical variable
5. Communicate a data comparison using clear and correctly labeled plots

---

## II. Dataset Overview (`board2.csv`)
The dataset contains student academic performance records consisting of the following features
* **Name**: Student identifier
* **Gender**: Student gender (`Male` / `Female`)
* **Track**: Academic track (`Instrumentation`, `Communication`, `Microelectron`)
* **Hometown**: Regional origin (`Luzon`, `Visayas`, `Mindanao`)
* **Subject Scores**: Numerical grades for `Math`, `Electronics`, `GEAS`, and `Communication`
* **Average**: Computed mean across all subject scores.

---

## III. Implementation Details

### **Part A: Visayas Communication DataFrame**
* Filters students whose `Hometown` is `Visayas` and `Track` is `Communication`
* Retains specified columns: `Name`, `Gender`, `Track`, `Hometown`, `Math`, `GEAS`, `Electronics`, and `Average`

### **Part B: Visayas Female DataFrame**
* Creates a focused DataFrame (`VisFemale`) for students whose `Hometown` is `Visayas` and `Gender` is `Female`
* Retains columns: `Name`, `Track`, `GEAS`, `Electronics`, and `Average`
* Filters a secondary view for students with an `Average` score of at least $60$ without mutating the primary DataFrame

### **Part C: Category-Average Visualization**
* Computes group means for the `Average` score categorized by `Track`, `Gender`, and `Hometown`
* Generates a unified figure containing three distinct, properly labeled bar charts with consistent scaling

---

## IV. Submission Requirements
* **File Format:** One Jupyter Notebook file (`.ipynb`) containing all code, outputs, visualizations, and interpretation statements
* **Execution:** All cells must execute from top to end without errors
