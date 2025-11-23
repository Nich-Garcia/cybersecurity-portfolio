# SQL Filtering Lab

## Overview
Queried and filtered data to identify suspicious activity, failed logins, and anomalies using SQL. This demonstrates foundational skills used in security investigations.

---

## 🔍 Example Query
```sql
SELECT * 
FROM logins
WHERE status = "FAILED"
ORDER BY timestamp DESC;
