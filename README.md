# Hospital Emergency Room Analysis Dashboard | Excel


## Project Overview
This project focuses on building an **Emergency Room (ER) Analytics Dashboard** using **Excel** to monitor patient flow, operational efficiency, and service quality.  
The dashboard enables hospital stakeholders to **identify bottlenecks, optimize wait times, and improve patient satisfaction** through data-driven insights.

---


## **Dashboard Preview**
![Hospital Dashboard Final  (1)](https://github.com/user-attachments/assets/b2cfa5c4-c191-4187-a62e-e1a878bbe3bc)


---

## Business Objective
- Monitor daily and monthly ER performance
- Track patient volume, wait times, and satisfaction
- Evaluate service timeliness and admission outcomes
- Identify trends across age groups, gender, and departments
- Support better operational and staffing decisions

---

## Project Workflow
1. Business Requirement Gathering  
2. Understanding ER Data  
3. Data Connection using **Power Query**  
4. Data Cleaning & Quality Checks  
5. Calendar Table Creation  
6. Data Modeling using **Power Pivot**  
7. DAX Calculations for KPIs  
8. Pivot Tables & Visual Design  
9. Dashboard Development  
10. Insight Generation  

---

## Key KPIs
| KPI | Description |
|---|---|
| **Number of Patients** | Daily ER patient count with trend analysis |
| **Average Wait Time** | Mean wait time before medical attention |
| **Patient Satisfaction Score** | Service quality indicator |
| **Timeliness %** | Patients attended within 30 minutes |
| **Admission Status** | Admitted vs Not Admitted |

---

## Visualizations Created
- KPI Cards with Sparklines  
- Patient Admission Status (Admitted vs Not Admitted)  
- Age Group Distribution  
- Gender-wise Patient Count  
- Patients Attended Within Time vs Delayed  
- Department Referral Analysis  
- Monthly Patient Trends  

---

## Data Modeling
- Star schema with **Fact & Dimension tables**
- Date-based analysis using a custom **Calendar Table**
- Optimized relationships for time intelligence

---

## Excel Calculations

### Age Group Classification

Age Group = IF([Patient Age] >= 70, "70-79", IF([Patient Age] >= 60, "60-69",IF([Patient Age] >= 45, "45-59",IF([Patient Age] >= 30, "30-44",IF([Patient Age] >= 15, "15-29",IF([Patient Age] >= 5, "05-14", "0-4"))))))

### Patient Timeliness Status

Attend Status =IF([Patient Waittime] < 30, "Within Time", "Delay")

### Calendar Table (Power Query)

= List.Dates(#date(2023,01,01), 731, #duration(1,0,0,0))

---

## Key Insights

- **61% of patients were attended within the target time (≤ 30 minutes)**, indicating generally effective ER response, with scope for improvement during peak hours.
- **Average wait time trends reveal congestion during high patient inflow days**, highlighting the need for better staffing and resource allocation.
- **Adults aged 30–44 formed the largest patient group**, making them the most frequent ER visitors.
- **Gender-wise distribution was nearly balanced**, suggesting no significant gender bias in ER visits.
- **General Practice and Orthopaedics received the highest referrals**, indicating higher demand for these departments.
- **Delayed cases showed strong correlation with higher daily patient volumes**, suggesting operational strain during busy periods.
- **Patient satisfaction scores fluctuated in line with wait times**, reinforcing that reduced delays directly improve service quality.

These insights help hospital stakeholders **identify bottlenecks, optimize ER workflows, and enhance patient experience** through data-driven decision-making.

---

## Tools & Technologies

- Power Query (M Language)
- Power Pivot
- Data Modeling
- Dashboard Design & Storytelling

---
## Business Impact

- Improved visibility into ER operations
- Enabled faster identification of service delays
- Supported capacity planning and workflow optimization
- Enhanced decision-making through real-time KPIsPower Query (M Language)

---

### Raw Data

The raw data file of Vrinda Stores can be downloaded from here:  
[`Hospital_Emergency_Room_Data.csv`](Hospital_Emergency_Room_Data.csv)


---


**Author:** *Kriti Dey*  
*Analyst*  
[LinkedIn](https://www.linkedin.com/in/kritidey/) · [GitHub](https://deykriti.github.io/)

---

