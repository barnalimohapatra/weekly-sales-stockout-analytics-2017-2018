• Infrastructure Layer: Multi-container isolation via Docker Compose (PostgreSQL DB + Independent Python Pipeline).
• Data Volume Persistency: PostgreSQL data must persist on the local host machine even if containers restart.
• ETL Automation: A standalone Python container that boots up, waits for the database, cleans messy raw currency fields, and runs a structured data load.
• Data Mart Layer: SQL views calculating week-over-week (WoW) revenue and customer transaction growth metrics.
• Semantic Connectivity: Port 5432 exposed to allow direct local analytical access via Power BI Desktop.
