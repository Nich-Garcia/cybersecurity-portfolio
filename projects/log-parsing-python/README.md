# Log Parsing & Python Automation

## Overview
Parsed system logs using Python to extract failed login events, anomalies, and suspicious patterns. This demonstrates foundational automation and log analysis skills commonly used in security operations.

---

## 🔧 Example Python Script
```python
import re

failed_attempts = []

with open("syslog.txt") as file:
    for line in file:
        if "FAILED LOGIN" in line:
            failed_attempts.append(line)

print(len(failed_attempts), "failed login attempts detected.")
