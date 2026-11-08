📅 Project Timeline: A Gantt Built by a Project Manager

I spent years coordinating projects before becoming a data analyst. This dashboard is the tool I wished I had: one view that shows what is late, by how many days, and where to act first.

Data is not there to impress. It is there to help a team decide faster.

Show Image Show Image Show Image

🎯 Objective

Project managers need to know one thing quickly: which tasks are late, and by how many days. This report turns a project schedule into a dynamic Gantt view that compares the baseline plan with the current forecast and surfaces schedule slip at phase, deliverable and task level.

Who it is for: project managers, PMO teams and stakeholders who follow a schedule but do not want to read a spreadsheet.

📊 Gantt View

Gantt

🔵 Light blue: planned dates (baseline)
🔷 Dark blue: forecast dates (current estimate)
🟥 Red square: milestone
Slip (days): delay of each task versus the plan
🔄 Project Lifecycle

Lifecycle

⏱️ Schedule Slip

Slip

📸 Power BI Report

Power BI Gantt

✨ Features
Hierarchy: Phase → Deliverable → Task
Planned vs. forecast bars on the same row
Slip (days) column to spot delays immediately
Milestone markers
Month-level time axis with a time slider
Columns: Version, Planned End, Forecast End, Slip (days)
🧮 Key Measure (DAX)
DAX
Slip (days) =
DATEDIFF ( MAX ( 'Tasks'[Planned End] ), MAX ( 'Tasks'[Forecast End] ), DAY )
🗂️ Data Model
Column	Description
Version	Phase / deliverable / task name
Planned Start / End	Baseline schedule
Forecast Start / End	Current estimate
Slip (days)	Forecast End − Planned End
🛠️ Tools

Power BI Desktop · DAX · Gantt custom visual

📂 Repository Structure
├── Project_Timeline.pbix
├── data/                 # sample data
├── images/               # banner, animated SVGs, screenshot
└── README.md
🚀 How to Use
Clone the repository
Open Project_Timeline.pbix in Power BI Desktop
Refresh the data and explore the timeline

⚠️ The data in this repo is sample data, not from a real client project.





👤 Author# Gannt-
Akram Brahem, Data Analyst (PL-300) LinkedIn
