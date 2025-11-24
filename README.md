<img width="1400" height="700" alt="best-movies-on-netflix" src="https://github.com/user-attachments/assets/b844db7e-5ebb-4bd8-9f49-c1d874e664e1" />


# Netflix-Data-Analytics-Pipeline-DBT-Snowflake
Designed an end-to-end ELT pipeline by extracting Netflix data from AWS S3 into Snowflake and applying modular transformations using DBT (raw, staging, and production layers). Further enhancement can be done using Airflow for automating the entire pipeline and visualising insights can be done using Looker Studio/Power BI.

Project Flowchart
<img width="1167" height="490" alt="netflix-dbt" src="https://github.com/user-attachments/assets/188193e6-681c-487d-8a12-943f03b75268" />

📊 Project Details
The pipeline processes Netflix data stored as a CSV file.

Extraction & Loading (EL)
Extract: Netflix CSV data is extracted and stored in Amazon S3.

Load: The data is loaded from Amazon S3 into Snowflake, specifically into the Raw Layer (1). This initial load is labeled "Raw Loading."

Transformation (T)
Tools: dbt (data build tool) is used for modular transformations, testing, and orchestration.

Transformation Flow: The raw data in Snowflake is transformed through dbt across two key layers:

Staging Layer (2): Data is processed in the Staging area of the Snowflake production database.

Serving Layer (3) / Production: The final, transformed data is stored in the Dev environment (serving layer) of the Snowflake database, ready for consumption.

Visualization & Enhancement
Visualization: The transformed data from Snowflake's serving layer is then used for visualization in popular BI tools like Looker Studio, Power BI, and Tableau.

Future Enhancement: The entire pipeline's automation is planned using Apache Airflow.

The architecture effectively uses AWS S3 for storage, Snowflake as the cloud data warehouse, and dbt for modern data transformations.


