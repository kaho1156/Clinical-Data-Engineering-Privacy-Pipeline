📌 Project Overview
This project is an End-to-End (E2E) Clinical Data Pipeline designed to automate hospital operational monitoring while maintaining strict patient privacy. It simulates a core Electronic Medical Record (EMR) environment, performing data synthesis, de-identification, and real-time KPI tracking.

💼 Professional Context
Inspired by my current role as a Ward Clerk at Alfred Health and my 6+ years of experience in financial compliance (HSBC, Bank of China), this system addresses the critical need for secure, data-driven decision-making in high-pressure clinical settings.

🚀 Key Features
Data Synthesis: Generates high-fidelity synthetic patient records including clinical specialties, admission sources, and financial identifiers.

Privacy-by-Design Engine: Implements advanced de-identification techniques to comply with the Privacy Act 1988 (Australia):

Masking: Redacts PII like names and Medicare numbers.

SHA-256 Hashing: Pseudonymizes Patient IDs to allow longitudinal analysis without identity exposure.

Generalization: Applies k-anonymity principles by grouping specific ages and birth years.

Operational Surveillance: A SQL-integrated monitoring layer to track hospital performance indicators.

📊 Clinical KPI Monitoring
The system monitors four core metrics critical to hospital administration and patient-centric care:

Patient Centricity (Upcoming Birthdays): Identifies patients celebrating birthdays within a rolling 72-hour window to enhance care experience.

Patient Flow (High Turnover): Surveillance of new admissions within the last 3 days to optimize ward clerk resource allocation.

Revenue Cycle Management (Private Fund Auditing): Identifies private insurance eligibility to ensure maximum hospital revenue recovery.

Bed Management (Long Stay Alert): Flags stays exceeding 14 days to assist management in identifying complex discharge planning needs.

🛠️ Technical Stack
Language: Python 3.12 (Pandas, Numpy)

Database: SQL (SQLite for in-memory processing)

Privacy: SHA-256 Cryptographic Hashing, Regex Masking

Simulation: Faker (en_AU locale)
