# 🛡️ SIEMsational CTF (Project 5)

This project is part of CodePath’s Cybersecurity curriculum and simulates a Capture-the-Flag (CTF) experience using Splunk as a Security Information and Event Management (SIEM) tool. The assignment involves analyzing structured data and threat indicators through search queries and visualization.

---

## 🚀 Project Overview

You’ll apply Splunk search, filtering, and statistics commands to:

- Investigate Netflix metadata to uncover insights on genres, ratings, and release years.
- Analyze suspicious behavior tied to malware file uploads and identify the attacker using log data.
- Use Splunk’s search processing language (SPL) to answer real-world security questions.

---

## 🧠 Skills Demonstrated

- 🕵️‍♂️ Log analysis and threat hunting
- 📊 Using Splunk SPL for data extraction and filtering
- 🔍 Identifying suspicious patterns and indicators of compromise (IOCs)
- 📂 Investigating structured metadata for trends

---

## 🔧 Tools Used

- Splunk (via the cyber101 Ubuntu VM in Azure Labs)
- Dataset: Netflix metadata and malware access logs
- Splunk SPL commands: `index`, `stats`, `table`, `search`, field filtering

---

## 📁 Project Structure

- `Netflix Questions`: Search queries to identify trends in Netflix's media catalog.
- `Malware Investigation`: Queries and analysis identifying attacker behavior and compromised systems.
- `Project 5 Submission Template`: Final answers submitted with corresponding SPL searches and screenshots.

---

## ✅ Sample Queries

```spl
index=main host="Netflix" type="TV Show" listed_in="*Docuseries*"
| stats count
