# Treemap Hierarchy for NHS Hospital AdmissionsPre- vs. Post-Pandemic Growth Rate Analysis

## 📊 Project Overview
"Visual Design Type": Hierarchical Treemap (Interactive Diverging Treemap)
"Tool Stack": Python (Plotly library)
"Focus Cohort": A comparative analysis of two critical periods:
"Pre-Pandemic Baseline": Average of 2018-2019
"Pandemic-Impacted Period": Average of 2020-2021
    
## 📉 Variables & Metrics
"Finished Consultant Episodes (FCE)": Chosen to accurately reflect actual hospital resource utilization.
"Growth Rate (%)": A direct comparison of 2020-21 vs. 2018-19 to highlight admission deviations caused by the pandemic shock.
## 🗺️ Visual Mappings
### A. Hierarchical Structure
The design features three parallel root-level branches for multi-dimensional exploration:
"1.Disease Category $\rightarrow$ Specific 3-character Diagnosis Codes."
"2.Gender $\rightarrow$ Gender Types $\rightarrow$ Respective Disease Summary Categories."
"3.Age Group $\rightarrow$ Age Segments $\rightarrow$ Respective Disease Summary Categories."
    
## B. Visual Encoding
"a. Size Mapping": The area of each rectangle is proportional to the Average Finished Consultant Episodes in 2020-2021. This allows users to immediately identify the highest-volume services and departments during the pandemic.
"b. Size:" The area of each rectangle is proportional to the Average Finished consultant episodes in 2020-2021, allowing users to immediately identify the highest-volume services.
"c. Color": Mapped to the Average Growth Rate using the BrBG_r diverging scale (-40% to +40%);
"d. Position": Uses a squarified algorithm where higher-volume nodes are positioned towards the top-left of each container for visual priority.
## 🗺️Unique Observation: 
The visualization reveals a stark "Healthcare Displacement" pattern. Widespread brown rectangles indicate a massive reduction in routine admissions, which most severely impacted the "Age 60+" vulnerable demographic. In sharp contrast, a massive teal-colored outlier (code U07: COVID-19) emerges in the "U" chapter, illustrating a dramatic surge that defied the general downward trend.
## 🗺️Data Preparation: 
"a. Missing Values": Masked counts (*) were imputed as 3 and nulls as 0 to enable accurate calculations.
"b. Anomalous Data": Inconsistent gender records were reclassified to "Unknown Gender" and special characters stripped to ensure flawless hierarchy mapping.

