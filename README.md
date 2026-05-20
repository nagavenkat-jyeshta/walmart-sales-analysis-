# 📊 Walmart Sales Data Analysis Dashboard

## 🧾 Project Overview
This project is an interactive data analysis dashboard for Walmart sales data. Built with a Python Flask backend and a PostgreSQL database, it automatically loads and structures raw CSV data into a robust relational database schema. The frontend provides dynamic, interactive charts (using Chart.js) allowing users to drill down into specific sales metrics.

## 🎯 Objectives
- Build a unified backend using Flask and PostgreSQL.
- Automatically load and normalize dataset (`walmart_sales.csv`) upon application startup.
- Implement complex database features including triggers, views, and stored procedures for efficient querying.
- Create an aesthetically pleasing, modern dashboard with interactive data drilldown capabilities.

## 🛠️ Technologies Used
- **Backend:** Python, Flask, `psycopg2`
- **Database:** PostgreSQL
- **Frontend:** HTML, CSS, Chart.js
- **Data Manipulation:** SQL (Triggers, Views, Stored Procedures)

## 📁 Project Structure
```text
walmart sales.pro/
│
├── template/
│   ├── app.py                   # Main Flask backend application
│   ├── walmart_sales.csv        # Dataset source file
│   ├── sql/
│   │   ├── schema.sql           # Database initialization (tables, triggers, procedures)
│   │   └── queries.sql          # Additional database analytical queries
│   └── templates/
│       └── index.html           # Frontend dashboard layout and logic
```

## 📌 Features
- **Automated Data Pipeline:** The Flask app reads `walmart_sales.csv` and uses PostgreSQL stored procedures (e.g., `InsertDeptSales`) to populate the database cleanly.
- **Interactive Drilldown:** Click on elements of the main graphs to reveal in-depth underlying data corresponding to that selection.
- **Consolidated SQL Scripts:** A centralized `schema.sql` makes it easy to tear down and rebuild the entire database infrastructure in seconds.
- **Beautiful UI:** A visually stunning dashboard, optimized for user experience.

## ⚙️ How to Run Locally

### Requirements
- Python 3.x
- PostgreSQL server running locally
- Required Python packages: `flask`, `psycopg2-binary`, `pandas`

### Setup Instructions

1. **Clone the repository:**
   ```bash
   git clone https://github.com/RaghuRamaKrishna24/WalmartSales-Data_Analysis.git
   cd "WalmartSales-Data_Analysis/template"
   ```

2. **Configure Database:**
   - Create a PostgreSQL database.
   - Run the `sql/schema.sql` file in your PostgreSQL client to set up all tables, views, and procedures.
   - Update your connection credentials in `app.py` if necessary.

3. **Install Dependencies:**
   ```bash
   pip install flask psycopg2-binary pandas
   ```

4. **Run the Application:**
   ```bash
   python app.py
   ```
5. **Access the Dashboard:**
   Open your browser and navigate to `http://127.0.0.1:5000/`.

## 🙋‍♂️ Author
**naga venkat jyeshta**  
[GitHub Profile](
