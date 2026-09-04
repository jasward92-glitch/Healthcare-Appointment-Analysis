# Healthcare Appointment Analysis

This project analyzes 100 healthcare appointments to identify patterns in patient wait times, satisfaction, appointment outcomes, provider performance, and billing.

The goal of this project was to transform raw healthcare appointment data into actionable insights through data cleaning, validation, descriptive analysis, Excel PivotTables, dashboard development, and Power BI visualization.

## Business Questions

This analysis focused on the following questions:

- What is the overall appointment completion rate?
- Which departments have the longest patient wait times?
- How does wait time vary by appointment type?
- How does patient satisfaction vary across departments and providers?
- Which providers show differences in wait time, satisfaction, and billing?
- What operational areas may benefit from further investigation?

## Tools Used

- Microsoft Excel
- Microsoft Power BI
- PivotTables
- PivotCharts
- Excel dashboards
- Power BI dashboards
- Data cleaning and validation
- Descriptive analysis

## Dataset

The dataset contains 100 healthcare appointment records.

Key fields include:

- Appointment ID
- Patient ID
- Patient Age
- Appointment Date
- Department
- Provider
- Appointment Type
- Appointment Site
- Insurance
- Appointment Time
- Wait Time
- Appointment Duration
- Status
- Satisfaction Score
- Referral
- Billing Amount

## Key Performance Indicators

| KPI | Result |
|---|---:|
| Total Appointments | 100 |
| Completion Rate | 94% |
| Average Wait Time | 34.47 minutes |
| Average Satisfaction | 3.82 / 5 |
| Average Billing | $290.95 |

## Key Findings

### Wait Time and Satisfaction

Department-level analysis showed an association between longer wait times and lower patient satisfaction.

- Orthopedics had the longest average wait time at **57.4 minutes** and an average satisfaction score of **2.5**.
- Cardiology had an average wait time of **56.3 minutes** and satisfaction of **2.6**.
- Pediatrics had the shortest average wait time at **11.3 minutes** and the highest satisfaction score at **5.0**.
- Primary Care averaged **22.57 minutes** of wait time with a satisfaction score of **4.3**.

These results suggest that longer wait times are associated with lower patient satisfaction, although the analysis does not establish causation.

### Appointment Type

Wait times varied considerably by appointment type.

- **New Patient:** 51.8-minute average wait across 28 appointments
- **Follow-Up:** 40.6-minute average wait across 32 appointments
- **Medication Check:** 27-minute average wait across 5 appointments
- **Annual Exam:** 22.7-minute average wait across 10 appointments
- **Sick:** 16.2-minute average wait across 15 appointments
- **Well Child:** 9-minute average wait across 10 appointments

New Patient and Follow-Up appointments represent important areas for further operational review because they combine relatively high appointment volume with longer average wait times.

### Provider Performance

Provider analysis compared average wait time, patient satisfaction, billing, and appointment volume.

Dr. Carter had the highest average satisfaction score at **4.35** across 28 appointments and an average wait time of approximately **22.5 minutes**.

Dr. Patel and Dr. Williams had the longest average wait times while also showing lower average satisfaction scores.

Average billing varied by provider, with Dr. Williams having the highest average billing amount at approximately **$458.50** and Dr. Carter having the lowest at approximately **$185.30**.

Billing differences should be interpreted alongside appointment type, services provided, insurance, and other factors rather than being treated as a standalone measure of provider performance.

### Appointment Status

Of the 100 appointments:

- **94 Completed**
- **3 Cancelled**
- **3 No-Show**

This resulted in an overall **94% completion rate**.

There were six blank satisfaction scores. These corresponded to the three cancelled and three no-show appointments. The blanks were intentionally preserved because no satisfaction response was available for appointments that were not completed.

## Recommendations

Based on the analysis, the following areas could be investigated further:

1. **Review patient flow in Cardiology and Orthopedics** to identify factors contributing to longer wait times.
2. **Evaluate New Patient scheduling** because this appointment type had the highest average wait time.
3. **Review Follow-Up scheduling capacity** because Follow-Up appointments represented the largest appointment category and also had relatively long waits.
4. **Monitor wait time and satisfaction together** to determine whether improvements in patient flow are associated with improved patient experience.
5. **Review practices in Pediatrics** to identify scheduling or workflow practices that may be useful in other departments.

## Data Quality

The dataset was reviewed for completeness and consistency before analysis.

Six satisfaction scores were blank because the corresponding appointments were cancelled or marked as no-shows. These values were not replaced with zero or an estimated score because doing so would misrepresent the underlying data.

Appointment counts were also validated across the major PivotTables and reconciled to the dataset total of 100 appointments.

## Excel Dashboard

The Excel analysis included KPI summaries and visualizations covering appointment volume, completion rate, wait time, satisfaction, billing, appointment status, and department-level performance.

The Excel workbook contains the cleaned dataset, analysis worksheets, PivotTables, and dashboard.

## Power BI Dashboard

The Power BI dashboard was created to provide a simplified interactive view of the healthcare operations analysis.

The dashboard includes:

- **Total Appointments:** 100
- **Completion Rate:** 94%
- **Average Satisfaction:** 3.82 / 5
- **Appointments by Department**
- **Average Wait Time by Department**
- **Department slicer for interactive filtering**

The dashboard allows users to filter the department and evaluate appointment volume, wait time, and satisfaction at a high level.

## Repository Contents

- `Healthcare_Appointment_Analysis.xlsx` — cleaned dataset, analysis worksheets, PivotTables, and Excel dashboard
- `Healthcare_Appointment_Analysis.pbix` — Power BI dashboard and visualization
- `README.md` — project documentation, analytical findings, and recommendations

## Conclusion

This project demonstrates the use of Excel and Power BI to clean, analyze, visualize, and communicate healthcare appointment data.

The analysis identified meaningful differences in wait times and satisfaction across departments and appointment types. The strongest opportunity for further investigation is improving patient flow in areas with longer wait times and lower satisfaction.

This project reflects a practical approach to healthcare data analysis by connecting operational metrics to patient experience and business decision-making.
