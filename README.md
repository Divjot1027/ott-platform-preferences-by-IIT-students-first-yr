# Student Preferences for OTT Platforms

**Description**  
Analyzes OTT platform preferences of 1st-year IIT Dhanbad students nationwide. Survey asked which single OTT subscription they'd choose if offered free, plus demographics and viewing habits. A dynamic Google Sheets pipeline feeds a Tableau dashboard visualizing platform/genre popularity, device & language trends, and weekly viewing.

**Live Links**  

- Google Form (data source):  https://docs.google.com/forms/d/e/1FAIpQLScX2B76nwODFdj3nXv-vkRqpU8dwgnobaFpeTdWApgTcPl7vA/viewform?usp=header
- Google Sheet (data source): https://docs.google.com/spreadsheets/d/1gsbP7POK5owBY3leEZKwTsqIH4c2InM2w4eVhvag4cs/edit?usp=sharing  
- Tableau Public dashboard: https://public.tableau.com/app/profile/divjot.singh3062/viz/StudentPreferencesforOTTPlatforms/OTTDashboard

---

## Contents
- `README.md` — project overview (this file)  
- `ott-dashboard.twbx` — packaged Tableau workbook (include if sharing)  
- `data/` — (optional) processed CSV(s) used by Tableau (anonymized)  
- `TRANSFORMS.md` — (optional) Google Sheets formulas / steps for preprocessing  
- `LICENSE` — suggested license files

---

## Data & pipeline
- **Collection:** Google Form responses stored in Google Sheets.  
- **Processing:** Dynamic helper tables in Google Sheets normalize and unpivot genre selections, create aggregates, and form a star schema (Responses fact table + Genres dimension).  
- **Visualization:** Tableau connects to the processed Google Sheet (or exported CSV). Tableau Public shows the published dashboard (link above). Note: Tableau Public refreshes linked Google Sheets approximately every 24 hours.

---

## Visuals (high level)
- KPIs: total respondents, avg age, gender split  
- OTT by language (pie)  
- OTT popularity (bar) — which platform students choose if given one free subscription  
- Genre popularity (bar) — unpivoted genre counts  
- Device × Language (stacked bars/treemap)  
- Weekly viewing frequency / hours (bar)  
- Demographic breakdowns (Genre by Gender, Genre by AgeGroup)  
- Respondent detail table for drilldowns

---

## Privacy
- Anonymize `Your Name` and any personally identifiable information before publishing data publicly.
---

## How to reproduce
1. Ensure your Google Sheet is accessible to the Google account used to connect with Tableau.  
2. In Tableau Public: Connect → Google Sheets → select the sheet → build / publish the dashboard.  
3. To update visuals immediately: refresh data in Tableau Desktop and re-publish. Tableau Public auto-refreshes ~24 hrs.

---

