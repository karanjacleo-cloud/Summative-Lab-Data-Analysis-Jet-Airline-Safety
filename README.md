#  Aviation Accident Analysis

## Project Overview
This project analyzes aviation accident data to understand patterns in passenger injuries across different aircraft types. The focus is on comparing **small vs large aircraft** using injury-related metrics.

---

## Objectives
- Analyze passenger injury outcomes in aviation accidents  
- Compare **injury fractions** between small and large aircraft  
- Identify patterns that may influence safety interpretation  

---

## Key Features / Variables
- `fatal_injury_fraction` → Proportion of passengers who died  
- `is_destroyed` → Whether the aircraft was destroyed (1 = Yes, 0 = No)  
- `total_passengers` → Total number of people onboard  
- `make_model` → Combined aircraft manufacturer and model  
- `weather_condition`, `engine_type`, `broad_phase_of_flight` → Contextual factors  

---

## 🧹 Data Cleaning Steps
- Standardized column names (lowercase, removed spaces, replaced dots)  
- Created new features:
  - `is_destroyed` (binary classification)
  - `make_model` (combined fields)
  - `fatal_injury_fraction` (ratio calculation)  
- Handled missing values and inconsistent formatting  

---

## 🔍 Key Insights

### 1. Small Aircraft
- Tend to have **higher injury fractions**
- Fewer passengers → higher proportional impact  
- Results can be **more extreme and variable**

### 2. Large Aircraft
- Show **lower injury fractions**
- Carry more passengers → lower proportional impact  
- More **stable and consistent patterns**

---

##  Important Observation
> Injury fractions alone can be misleading.

- Small aircraft may appear riskier due to high percentages  
- Large aircraft may seem safer despite higher total injuries  


---

##  Conclusion
Small aircraft show higher proportional risk, while large aircraft distribute risk across more passengers. A complete safety analysis must combine both **percentage-based metrics** and **total counts** to avoid incorrect conclusions.

---

## Tools Used
- Python  
- Pandas  
- Matplotlib / Seaborn  
- Jupyter Notebook / VS Code  

---

## Files
- `Aviation_Accidents_Cleaning.ipynb` → Data cleaning & preprocessing  
- `Summative_Analysis.ipynb` → Analysis and insights  


