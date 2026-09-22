# Experiment 4: Data Wrangling and Data Visualization


## I. Intended Learning Outcomes
At the end of this laboratory activity, the student is able to:
1. Filter tabular data using several categorical and numerical conditions[cite: 1].
2. Construct focused DataFrames by selecting relevant features[cite: 1].
3. Summarize the relationship between categorical features and a numerical variable[cite: 1].
4. Communicate a data comparison using clear and correctly labeled plots[cite: 1].

---

## II. Dataset Overview (`board2.csv`)
The dataset contains student academic performance records consisting of the following features[cite: 2]:
* **Name**: Student identifier[cite: 2]
* **Gender**: Student gender (`Male` / `Female`)[cite: 2]
* **Track**: Academic track (`Instrumentation`, `Communication`, `Microelectron`)[cite: 2]
* **Hometown**: Regional origin (`Luzon`, `Visayas`, `Mindanao`)[cite: 2]
* **Subject Scores**: Numerical grades for `Math`, `Electronics`, `GEAS`, and `Communication`[cite: 2]
* **Average**: Computed mean across all subject scores.

---

## III. Implementation Details

### **Part A: Visayas Communication DataFrame**
* Filters students whose `Hometown` is `Visayas` and `Track` is `Communication`[cite: 1].
* Retains specified columns: `Name`, `Gender`, `Track`, `Hometown`, `Math`, `GEAS`, `Electronics`, and `Average`[cite: 1].

### **Part B: Visayas Female DataFrame**
* Creates a focused DataFrame (`VisFemale`) for students whose `Hometown` is `Visayas` and `Gender` is `Female`[cite: 1].
* Retains columns: `Name`, `Track`, `GEAS`, `Electronics`, and `Average`[cite: 1].
* Filters a secondary view for students with an `Average` score of at least $60$ without mutating the primary DataFrame[cite: 1].

### **Part C: Category-Average Visualization**
* Computes group means for the `Average` score categorized by `Track`, `Gender`, and `Hometown`[cite: 1].
* Generates a unified figure containing three distinct, properly labeled bar charts with consistent scaling[cite: 1].

---

## IV. Submission Requirements
* **File Format:** One Jupyter Notebook file (`.ipynb`) containing all code, outputs, visualizations, and interpretation statements[cite: 1].
* **Execution:** All cells must execute from top to end without errors[cite: 1].
