 # 🏁 Formula 1 Racing Data Analysis using Azure and Databricks

This project offers a deep-dive analysis of Formula 1 racing trends by building a fully automated data pipeline using Azure services and Databricks. By integrating real-time data from the Ergast Developer API, the project delivers interactive dashboards that highlight driver and team performance over time.

---

## 📌 Project Highlights

- 🔁 **Automated Data Pipeline**: Built using Azure Data Factory to continuously extract racing data from the Ergast Developer API and store it in Azure Data Lake.
- 🚀 **Scalable Cloud Architecture**: Utilized Azure Databricks and Delta Lake for big data processing and SQL-based analytics.
- 📊 **Interactive Dashboards**: Developed in Databricks to visualize team dominance, driver stats, and performance shifts across seasons.
- 🔍 **Historical Insights**: Analyzed key transitions in the F1 landscape—from the Williams era to the rise of Red Bull and Mercedes.

---

## 🏗️ Architecture Overview

```text
Ergast API → Azure Data Factory → Azure Data Lake → Azure Databricks (PySpark + SQL) → Dashboards
```

### 🔹 1. Data Ingestion
- Data is pulled via API using Azure Data Factory on a scheduled basis.
- Raw race, driver, and constructor data is stored in Azure Data Lake Storage.

### 🔹 2. Data Processing
- Performed within Databricks using PySpark.
- Includes cleaning, normalization, transformation, and schema modeling.
- Converted to structured Delta tables with support for ACID transactions.

### 🔹 3. Analysis
- SQL queries power analytical views like:
  - Top drivers by total wins and podium finishes
  - Constructor performance across decades
  - Shift in dominance between teams and eras

### 🔹 4. Visualization
- Dashboards showcase:
  - Driver and team dominance over time
  - Performance trajectories through time-series plots
  - Anomalies and strategic shifts in motorsport competition

---

## ⚙️ Tech Stack

| Category              | Tools & Services                          |
|-----------------------|-------------------------------------------|
| Cloud Infrastructure  | Azure Data Lake Storage, Azure Databricks |
| Data Orchestration    | Azure Data Factory                        |
| Programming Language  | Python (PySpark), SQL                     |
| Data Modeling         | Delta Lake Tables                         |
| Visualization         | Databricks Dashboards                     |

---

## 🔍 Example Insights

- 📈 **Performance Shifts**: Visualization shows how dominant teams evolved from Williams in the 90s to Red Bull and Mercedes in recent years.
- 🧠 **Strategic Value**: These insights could inform racing strategies, fan engagement analysis, or sponsorship decisions.

---

## 📦 Folder Structure

```text
Formula-1/
├── ingestion/            # API ingestion notebooks/scripts
├── processing/           # Data transformation logic (PySpark)
├── sql_queries/          # SQL scripts for analytics
├── dashboards/           # Visualization notebook exports
├── dataset/              # Raw and transformed datasets
├── diagrams/             # Project architecture diagrams
└── README.md             # Project overview and documentation
```

---

## 📈 Future Enhancements

- Real-time ingestion using Azure Event Grid and Azure Functions
- Integration with Power BI for advanced visual storytelling
- Add predictive modeling for race outcome forecasting

---

## 🤝 Acknowledgements

- **[Ergast Developer API](https://ergast.com/mrd/)** for the Formula 1 dataset
- Microsoft Azure for cloud infrastructure
- Databricks for scalable analytics and visualization

---

## 📬 Contact

For any queries, suggestions, or collaborations, feel free to reach out via [GitHub](https://github.com/Akuljoshi).

---
