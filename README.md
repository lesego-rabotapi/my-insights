My-Insights: MyCiTi Data Dashboard

A full-stack data visualization application designed to provide actionable insights into the MyCiTi public transport network. This project leverages a Python-based web interface to interact with a relational database, transforming raw transit data into interactive maps and searchable tables.
Overview

My-Insights is a specialized dashboard built to help users and planners visualize MyCiTi routes, stop locations, and system-wide data. By connecting a high-performance MySQL backend with a Streamlit frontend, the application provides a seamless experience for spatial data analysis.
Tech Stack

    Frontend: Streamlit (Python Framework)

    Backend: MySQL

    Language: Python 3.x

    Data Visualization: Pandas, Folium/Streamlit Map components

    Database Connectivity: mysql-connector-python or SQLAlchemy

Key Features

my-insights/
├── app.py              # Main Streamlit application logic
├── database/           # SQL scripts for schema creation and data seeding
├── requirements.txt    # Python dependencies
└── README.md


Setup & Installation
1. Prerequisites

    Python 3.8+

    MySQL Server installed and running

2. Database Configuration

    Create a new MySQL database.

    Import the provided schema (if available in /database) or ensure your tables for routes and stops are populated.

    Update the database connection string in app.py:

    Interactive Geospatial Mapping: Visualize all MyCiTi stop locations across the city on an interactive map.

# Example config
DB_CONFIG = {
    "host": "localhost",
    "user": "your_username",
    "password": "your_password",
    "database": "myciti_db"
}

# Clone the repository
git clone https://github.com/lesego-rabotapi/my-insights.git

# Navigate to the project directory
cd my-insights

# Install dependencies
pip install -r requirements.txt

# Run the dashboard
streamlit run app.py
