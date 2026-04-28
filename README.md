### Treemap-Hierarchy for NHS Hospital Admissions: Pre- vs. Post-Pandemic Growth Rate
##●	Visual Design Type: Hierarchical Treemap (Interactive Diverging Treemap)
##●	Name of Tool: Python (Plotly library)
##●	Focus Cohort: A comparative analysis of two periods: the pre-pandemic baseline (Average of 2018-2019) versus the pandemic-impacted period (Average of 2020-2021).
##●	Variables: Finished Consultant Episodes (FCE): Chosen to accurately reflect actual hospital resource utilization; Growth Rate (%): Compares 2020-21 vs. 2018-19 to highlight admission deviations caused by the pandemic shock.
##●	Visual Mappings: 
#a. The design features three parallel root-level branches:
#-- Disease Category -> specific 3-character Diagnosis Codes. 
#-- Gender -> Gender types -> their respective Disease Summary Categories. 
#-- Age Group -> Age segments -> their respective Disease Summary Categories.
#b. Size: The area of each rectangle is proportional to the Average Finished consultant episodes in 2020-2021, allowing users to immediately identify the highest-volume services.
#b. Size: The area of each rectangle is proportional to the Average Finished consultant episodes in 2020-2021, allowing users to immediately identify the highest-volume services.
#b. Size: The area of each rectangle is proportional to the Average Finished consultant episodes in 2020-2021, allowing users to immediately identify the highest-volume services.
#c. Color: Mapped to the Average Growth Rate using the BrBG_r diverging scale (-40% to +40%);
#d. Position: Uses a squarified algorithm where higher-volume nodes are positioned towards the top-left of each container for visual priority.
#● Unique Observation: The visualization reveals a stark "Healthcare Displacement" pattern. Widespread brown rectangles indicate a massive reduction in routine admissions, which most severely impacted the "Age 60+" vulnerable demographic. In sharp contrast, a massive teal-colored outlier (code U07: COVID-19) emerges in the "U" chapter, illustrating a dramatic surge that defied the general downward trend.
#● Data Preparation: 
#a. Missing Values: Masked counts (*) were imputed as 3 and nulls as 0 to enable accurate calculations.
#b. Anomalous Data: Inconsistent gender records were reclassified to "Unknown Gender" and special characters stripped to ensure flawless hierarchy mapping.

