# Uber_DATA_ANALYSIS-on-Snowflake

## Tools & Technologies Used:
    AWS S3: For cloud-based data storage
    Snowflake: For data warehousing, SQL queries, and advanced analytics
    SQL: For querying, transformation, and segmentation
    Snowflake External Stage Integration: To link Snowflake with S3


# Workflow:
1. Data Upload to AWS S3:
  Raw Uber trip data was uploaded into an S3 bucket.

2. Connecting S3 to Snowflake:
    Created a Storage Integration in Snowflake.
    Configured the IAM role and trust policies to allow Snowflake access to S3.

 3. Creating External Stage:
    Established a stage in Snowflake pointing to the S3 bucket.
    Verified the connection and file availability using LIST and SELECT commands.

4. Loading Data into Snowflake Table:
    Defined a file format (CSV) and created an empty table matching the schema.
    Loaded data using the COPY INTO command from the external stage.

5. Data Analysis on Uber Trips:
    Performed various SQL analyses including:
    Time interval segmentation (e.g., short, medium, long rides)
    Time-of-day booking trends (Morning, Afternoon, Evening, Night)
    Fare and surge fee-based revenue breakdowns
    Ride count distribution and duration-based categorization


# Key Insights Derived
  Identified peak booking hours and corresponding revenue contribution.
  Categorized trip durations to find frequency and revenue by ride length.
  Generated time-of-day analytics to understand user behavior patterns.
  Pareto Analysis on what locations contributes 80% of Total Revenue.


# What This Project Demonstrates
  Real-world usage of cloud data integration (S3 → Snowflake)
  Data loading, staging, and transformation in Snowflake SQL
  Ability to build and analyze large datasets using SQL queries
  Skills in handling external cloud storage and Snowflake access management
