# 📊 Analytics Engineering Project Using Northwind Data

# 🌟 Project Overview
This project focuses on building an end-to-end analytics solution using the Northwind sample data. By leveraging Google BigQuery and dbt (Data Build Tool), we implemented a scalable 3-tier Data Architecture. The final product is a robust data pipeline integrated with Google Data Studio for effective data visualization and reporting.

# Key Highlights:
Data Architecture: 3-tier consisting of Data Lake, Staging, and Data Warehouse layers.
Transformation: Utilized dbt to move and transform data across layers.
Visualization: Built a One Big Table (OBT) model for simplified data consumption and reporting.
Dashboarding: Leveraged Google Data Studio for interactive visualizations.

# 🛠️ Tools & Technologies
SQL: For querying and managing data in BigQuery.
dbt: For transforming data across different layers of the architecture.
BigQuery: To store and query the Northwind data.
Looker Studio: (formerly Google Data Studio) for building interactive dashboards.
Excel: Used initially for data profiling.

# 📚 Key Skills Acquired
Data Profiling: Understanding the structure, content, and quality of data before transformation.
Bus Matrix Creation: Designed a bus matrix to map out the relationship between facts and dimensions.
Data Warehouse Dimensional Modeling: Applied Kimball methodology to design star and snowflake schemas.
dbt Development & Debugging: Wrote transformation scripts, tested models, and debugged errors efficiently.
BigQuery Configuration: Configured datasets, optimized queries, and managed access permissions in Google BigQuery.

# 🚀 Project Structure
1. Data Architecture
Data Lake Layer: Raw Northwind data ingested from source files (CSV/JSON) and stored in BigQuery.
Staging Layer: Transformation of raw data into intermediate tables with cleaned data.
Data Warehouse Layer: Final layer with star schema structure for analytics and reporting.
2. ETL Process
dbt: Managed transformations using a series of dbt models, staging data, and building the final reporting tables.
Staging Models: _stg models clean and prepare data.
Core Models: Fact and dimension tables.
OBT (One Big Table): A wide table that consolidates key business metrics.
3. Data Visualization
Google Data Studio: Connected the OBT to Looker Studio for data exploration and dashboard creation.
Key Visuals: Sales trends, top customers, product performance, etc.

# 📂 Folder Structure
bash
Copy code
├── dbt_project.yml              # dbt project configurations
├── models/                      # dbt models for transformations
│   ├── staging/                 # Raw to staging transformations
│   ├── core/                    # Core transformations (fact & dimension tables)
│   ├── marts/                   # Business metrics, One Big Table
├── data/                        # Initial data (Northwind CSVs)
├── dashboards/                  # Google Data Studio links/screenshots
├── README.md                    # Project documentation (this file)
