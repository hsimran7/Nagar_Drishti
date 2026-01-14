NagarDrishti AI: Smart City Reporting System
NagarDrishti AI is a professional civic engagement platform that connects citizens with government authorities. It allows residents to report local issues like potholes, garbage, or water leaks, while providing government officials with an AI-prioritized dashboard, live geospatial maps, and interactive drill-down analytics.

 Key Features
 For Citizens
Intuitive Reporting: A simple, modern form to report civic issues with category selection.

Geographic Tracking: Citizens provide precise addresses to ensure maintenance teams can find the location.

Real-time Status: A personal "My Reports" dashboard to monitor whether a complaint is Pending or Resolved.

 For Government Officials
AI Critical Path: A specialized "Dispatch Center" that automatically highlights High Severity unresolved issues at the top of the dashboard.

Live Geospatial Map: An interactive map using Leaflet.js that plots complaints as markers (Red for High severity, Blue for others).

Interactive Drill-Down Analytics:

Main View: A professional bar chart showing total complaints per neighborhood.

Drill-Down View: Click any neighborhood bar to instantly generate a detailed doughnut chart of specific problems (e.g., how many potholes vs. garbage issues) in that area.

 Tech Stack
Backend: Python / Flask

Database: SQLite (Optimized with sqlite3.Row for fast data retrieval)

Frontend: HTML5, CSS3 (Custom modern UI), Jinja2 Templating

Visualizations: Chart.js (Interactive Drill-down logic)

Maps: Leaflet.js (Geospatial data visualization)

 Analytics Logic
This project moves beyond simple lists by using a multi-dimensional data approach

/NagarDrishti-AI
├── app.py
├── civic.db
├── README.md
├── requirements.txt
├── static/
│   ├── styles.css
│   └── uploads/
└── templates/
    ├── citizen/
    └── government/

Data Cleaning: The backend converts SQLite rows into standard Python dictionaries to ensure 100% safe JSON serialization for the frontend.

Neighborhood Recognition: The system uses a specific logic to scan address strings and accurately group them into defined city neighborhoods (e.g., Model Town, Sardar Nagar).

Dynamic Filtering: JavaScript listeners detect user clicks on graphs to filter and re-render data without reloading the page.
