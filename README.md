####Hospital Patient Care & Operational Analysis
1. Purpose
The Hospital Patient Analysis Dashboard is an end-to-end data analytics solution designed to optimize healthcare delivery across 101,766 patient records. It provides stakeholders with actionable insights into clinical resource utilization, patient risk stratification (acuity), and operational efficiency to improve staffing and patient outcomes.

2. Tech Stack
Python (pandas/seaborn): Used for data cleaning, calculating clinical metrics, and initial exploratory data analysis (EDA).
MySQL: Utilized for structured data storage and complex queries regarding re-admission logic and patient history.
Power BI: The primary visualization platform for the interactive Healthcare Performance Dashboard.
Feature Engineering: Created metrics such as acuity_score, nurse_required_count, and historical_loss to track hospital resource impact.

3. Dataset Summary
The dataset contains 101,766 rows and 49 columns covering the full spectrum of a patient's hospital journey:
Demographics: Age, Gender, and Race.
Clinical Details: Time in Hospital, Number of Lab Procedures, Number of Medications, and A1C Results.
Operational Metrics: Admission Type (Emergency/Elective), Discharge Status, and Payer Code.
Medication Data: Tracking changes in 23 different medications including Insulin and Metformin.

4. Key Business & Clinical Insights
A. Efficiency & Demographics
Length of Stay (LoS): The average time in hospital is 4.40 days. Patients in the 70-80 age group represent the highest volume of admissions.
Clinical Intensity: On average, a patient undergoes 43.1 lab procedures and is prescribed 16.0 medications per visit.
Acuity & Staffing: High-acuity patients directly correlate with increased nurse_required_count, identifying a need for specialized staffing in high-risk wings.

B. Medication & Loyalty (Re-admission)
Diabetes Impact: 77% of patients are on diabetes medication.
Re-admission Trends: Patients on diabetes medication show a higher average rate of inpatient visits (0.65) compared to non-medicated patients (0.57).
Care Gaps: A significant portion of "Frequent Flyer" patients (high inpatient counts) are linked to specific medical specialties like Internal Medicine.

C. Financial & Operational Trends
Historical Loss: The 70-80 age bracket accounts for the highest historical loss ($41.4M), followed by the 80-90 group ($28.1M), highlighting where cost-containment strategies are most needed.
Admission Source: Emergency admissions have a significantly higher clinical complexity compared to elective admissions.
Lab Utilization: There is a strong positive correlation between the number of lab procedures and the total time spent in the hospital.

5. Business Recommendations
Targeted Geriatric Care: Develop specialized care protocols for the 70-90 age demographic to reduce historical loss and optimize resource usage.
Chronic Disease Management: Implement a post-discharge follow-up program specifically for patients on diabetes medication to lower the 0.65 re-admission average.
Staffing Optimization: Use the nurse_required_count and acuity_score trends to automate weekly staffing schedules, ensuring high-risk shifts are never under-resourced.
Operational Streamlining: Review lab procedure protocols for patients staying over 5 days to identify redundant testing and reduce the "Time in Hospital."

6.Demo :- The demo of dashboard is :  <img width="1920" height="1080" alt="Snapshot of dashboard" src="https://github.com/user-attachments/assets/aef2dbfa-0a30-451a-851f-89113ec2308c" />
