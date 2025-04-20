In this Project, I have used multiple GCP services to perform ELT on Global Health data CSV file and loaded the file into GCS bucket, utilized Airflow deployed on VM instance and loaded the CSV file into Staging dataset table.
Then transformed the data into multiple tranformed tables by splitting the raw data into multiple tables by country type.
Lastly, created views by modifying the column names and filtering the data as per the requirements and populated view for each country table
Resource: Vishal Bulbule resources has been used to understand and perform end to end data engineering project, Thanks Vishal for great resource

GCP Services used:
1. GCS: Google Cloud Storage
2. BQ: Big Query
3. VM Instance: To Install Airflow and perform ELT
5. Looker: For Reporting and Scheduling

**Data Flow Architecture**
![image](https://github.com/user-attachments/assets/7e15d0f1-8d9a-4233-af83-69fe61e5c1f4)

**GCS Bucket Details**

![Source_GCS_Bucket_1_Million_Records_CSV_File](https://github.com/user-attachments/assets/480adcc7-6143-463c-b692-ba64998ef754)

**Big Query Datasets and Tables Information**

![BigQuery_Tables_Views_Information](https://github.com/user-attachments/assets/57fa4223-3384-4672-9567-a23ea49d9d54)

**Complete Airflow GCS to BQ Tables and View DAG:**

![Final_GCS_Bucket_To_BigQuery_Tables_to_BigQuery_Views_Airflow_DAG_Flow](https://github.com/user-attachments/assets/25fe930a-747e-428a-927e-b02271af7ae8)

**Looker Report**

![Looker_Reporting_Web_UI](https://github.com/user-attachments/assets/82b4b9b9-39e0-4afc-ae8c-8e7135e32459)

Looker PDF Report URL: https://github.com/ViinayKumaarMamidi/Airflow_GCP_Data_Engineering_Project/blob/main/India_Health_Data_Report.pdf


**Looker Report Subscriptions/Scheduling**
Scheduled the report to be sent daily at 4 PM EST

![Looker_Report_Email_Attachment](https://github.com/user-attachments/assets/0f75fa31-a67c-4cb9-967a-c2cf0754da84)




