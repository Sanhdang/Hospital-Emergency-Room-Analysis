# Hospital-Emergency-Room-Analysis
A Power BI dashboard for an Emergency Room that consolidates 9,216 encounters (Apr-2023 → Oct-2024) into actionable KPIs and visuals. It tracks Average Wait Time (35.3 min), Patient Satisfaction (4.99/10), % Seen ≤30 Minutes (59.32%), Admissions vs. Non-Admissions, demand by day/hour, demographics (age, gender, race), and referral destinations
## 📌 Project Overview
This project explores ED operational data to uncover patterns in arrival demand, patient flow (from registration to disposition), patient experience, demographics, and referral pathways.
Using data modeling, DAX measures, and thoughtful visualization, the goal is to help teams staff smarter, reduce waits, and coordinate beds/consults more smoothly.
It’s a fun, curiosity-driven topic I want to build and learn from while practicing data storytelling in healthcare.

## 🎯 Objectives
Identify demand peaks by weekday and hour for demand-shaped staffing.

Track flow performance (intake → triage → first clinical contact → diagnostics → disposition) and surface bottlenecks.

Connect wait dynamics with patient satisfaction to guide service-recovery actions.

Profile patient mix (age, gender, race) to support inclusive service design.

Map referral/consult destinations to standardize fast-track pathways.

Provide practical recommendations and a governed, reusable Power BI model.

## 🗂️ Dataset
ED encounter data: ArrivalDateTime, RegistrationDateTime, TriageStart, FirstContactDateTime, Disposition, AdmissionFlag, ObservationFlag.

Experience data: SatisfactionScore (survey).

Demographics: AgeBand, Gender, Race (de-identified).

Referral destinations: normalized ReferralDept.

Cleaning & preprocessing via Power Query; modeling and measures in Power BI.

## 🔬 Methodology
Data Cleaning & Standardization – unify time zones, handle outliers, normalize labels.

Star Schema Modeling – FactER with DimDate, DimPatient, DimDepartment.

Core DAX Measures – wait time, on-time first contact, admissions, referrals, satisfaction.

Visualization & UX – blue theme, accessible fonts, plain-English tooltips, drill-through.

Governance – metric definitions, assumptions, and caveats documented in-report.

## ✅ Expected Outcomes
Clear view of when pressure builds and where flow stalls.

Actionable insights for staffing, fast-track protocols, and bed coordination.

A tidy, reusable Power BI asset that’s easy to iterate as new questions arise.
