## ETL Process (SSIS)

### Data Sources
- CSV files: `employees.csv`

### ETL Logic
- Data Cleaning: Remove nulls, trim fields, and validate data types
- Type Conversion: Convert string to `int`, `datetime`, etc.
- Lookup Transform: Map `city_id` to full city names
- Error Handling: Script component logs bad rows to CSV with row-level error messages
- File Handling: Archive processed files and log row counts (valid/invalid) to a tracking table

---

## 📊 Power BI Dashboard

### 👥 Report: HR Overview
**SQL Server Data Source:** `Employees`, `Departments`

**KPIs:**
- Total Employees
- Average Salary
- Employee Distribution by Department

**Visuals Used:**
- Bar Charts (Headcount by Dept)
- Maps (Office Location Distribution)
- Filters: Location, Department, Salary Range

---

## Tools & Technologies

| Component | Tools Used |
|----------|------------|
| ETL | SSIS (SQL Server Integration Services) |
| Database | SQL Server |
| BI Reporting | Power BI |
| Scripting | Script Component in SSIS |
| Version Control | GitHub |

## Key Learnings

- Building reusable ETL pipelines for structured CSV ingestion
- Handling bad data rows without breaking the ETL flow
- Translating raw transactional data into business insights via Power BI

  
