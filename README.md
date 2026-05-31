Medical Appointment Data Cleaning

Rows: 110,527

Columns: 14

Cleaning Steps Performed
Checked the dataset for missing values and duplicate records. No missing values or duplicate records were found.
Applied AutoFit Column Width and AutoFit Row Height to improve the readability of the dataset.
Filtered the Age column and found a negative age value. Since negative age is not valid, that record was removed. Ages such as 100, 102, and 115 were kept in the dataset and considered as potential outliers.
Corrected two incorrect column names:
Hipertension → Hypertension
Handcap → Handicap
Created a new column called Waiting_Days to calculate the difference between the appointment date and the scheduled date.

Created a new column called Total_Conditions to calculate the total number of health conditions for each patient using:

=[@Hypertension]+[@Diabetes]+[@Alcoholism]+[@Handicap]

New Columns Created
Waiting_Days
Total_Conditions
Final Outcome

The dataset was cleaned and validated by checking data quality issues, correcting column names, removing invalid records, and creating additional columns that can be used for further analysis and reporting.