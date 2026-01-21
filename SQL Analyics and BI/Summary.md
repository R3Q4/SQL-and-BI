# SQL and BI Course Notes

# 

### Overview of Databrick functions
Databricks simplifies the complexity in data estate, reducing unecessary cost from multiple copies of data, break free from lock-in with open format

1. Unity Catalog: data stored in an open, broadly accessible lakehouse format
2. lakeflow: ingest, ETL, streamline
3. Databrick SQL: data warehousing
4. AI/BI: business intelligence
5. Mosaic AI: artificial intelligence 

#### Features : unified capabilites for each use case
1. security: tables - access control, auditing
2. collaboration - AI models - discovery, secure open sharing
3. quality - files - lineage, quality monitoring
4. insights - dashboards - control costs, business semantics

- Lakeflow: reliable and auomated dataflow from systems-of-records
    + connect easily to key data sources
    + datapipelines made easy
- Databrick Warehouse: data storage with complete warehouse capabilites
    + lower cost of migration 
    + foundational functionality + governance and administration
- AI/BI : intelligent analytics for real-world data
    + results with AI powered understanding
- Mosaic AI: domin specific agentic applications
    + prepare data: data ingestion, ML features, vector index
    + build agents: gen AI models, classifcal ML models, function and tools
    + deploy agents: agent serving, MLOps/LLMOps, lineage
    + evaulate agents: LLM judge, peer labeling, tracing
    + govern data: AI guardrails, credentials, rate limits, usage tracking

#### How it works
General Intelligence; large model trained on entire web leveraging scaling laws
Data Intelligence: AI agents that reason on your data and solve domain specific problem
Delta lake: open source protocol for reading and writing files to cloud storage
- data sources -> ingestion -> lakehouse
    + key features: ACID Transaction - guarantees table level to data stored in cloud based object storage (atomicity, consistency, isolation, durability)
        + atomicity: entire transaction completes
        + consistency: data follow rules or will be rolled back
        + isolation - one transaction completed before start of another
        + durability - data saved in a persistent state once completed
    + Data operation: insert, update, delete, merge
    + time travel: query historical data, restore previous versions
    + Schema enforcement: adjust schema of delta table as data changes
#

### Data Analytics
Key Responsibilities of Data Analytics
1. data collection, cleaning and processing: define problem to be solved curate and select data needed to solve the situation, clean and process data in conjunction with data engineers
2. exploratory Data Analysis: understand data's characteristics, patterns, trends and outliers; develop hypothesis and summary statistics
3. Data Modeling, Analysis and presentation: use visualisations, dashboards and other methods to present findings and conclusions

Common Challenges of making data warehousing and BI so difficult
1. data silos and multiplesystem
    + needed data scattered across multiple platforms
    + data teams operate in silos using inconsistent datasets
2. Data Quality
    + Data lakes and warehouses have limitation
    + getting cleaned data is time consuming and delays insights 
3. Governance and Compliance
    + each platform in the ecosystem has a different governance structure
    + managing sensitive data is complicated in a disjoint system

Data Warehouse VS Data Lakes
- data warehouse for BI: clean data, reports, Ad Hoc Queries, data exploration
- Data Lake for AI: predictive modeling, prescriptive analytics, automated decision making

### Architecture for Databricks Intelligence platform
- data sources -> ingest -> transform -> qiery -> visualise -> serve -> external apps
- governance and security + unified storage layer

Benefits of Databricks SQL
- provides unified streaming and batch processing environment
- databricks SQL is enterprise ready -> can use it for production workloads
- all-in-one environment: simpler to administer

AI/BI dashboards
- all-in-one visualisation and presentation environment
- native performance optimisation allow for near instant interactivity at scale
- share for organisation and reviews
dataset -> data -> visualisation (chart and filters)