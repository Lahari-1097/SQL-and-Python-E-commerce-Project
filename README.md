# 🛒 E-Commerce Data Analytics Project (Python + SQL)

## 📌 Overview
This project demonstrates an end-to-end **Data Analytics workflow** using **Python, MySQL, and SQL**.  
The objective is to load multiple e-commerce CSV datasets into a relational database and perform business-driven SQL analysis.

### Workflow
Raw CSV Data → Python ETL Script → MySQL Database → SQL Analysis → Business Insights

---

## 📂 Project Structure

```
├── csv_to_sql.py                # Python ETL script to load CSV files into MySQL
├── python+sql_ecommerce.ipynb   # SQL analysis notebook
├── Questions.txt                # Business SQL questions
├── dataset_link.txt             # Dataset download link
└── README.md
```

---

## 📊 Dataset

Download dataset from:

https://drive.google.com/drive/folders/12dvYxsUZ7XUwlrXn6NTz6wwt7-0mdHsV?usp=sharing

After downloading, place all CSV files inside one folder.

Expected files:

- customers.csv  
- orders.csv  
- sales.csv  
- products.csv  
- delivery.csv  
- payments.csv  

---

## 🧰 Tech Stack

- Python
- Pandas
- MySQL
- SQL
- Jupyter Notebook

---

## ⚙️ ETL Process (Python → MySQL)

The script **csv_to_sql.py** performs:

- Reads CSV datasets using pandas
- Cleans column names automatically
- Detects SQL data types dynamically
- Converts missing values to SQL NULL
- Creates tables automatically
- Inserts records into MySQL database

Tables created:

- customers
- orders
- sales
- products
- delivery
- payments

---

## 🚀 Setup Instructions

### 1. Clone Repository

```bash
git clone https://github.com/your-username/ecommerce-sql-project.git
cd ecommerce-sql-project
```

### 2. Create Virtual Environment

```bash
python -m venv .venv
```

Activate environment:

**Windows**
```bash
.venv\Scripts\activate
```

**Mac/Linux**
```bash
source .venv/bin/activate
```

---

### 3. Install Dependencies

```bash
pip install pandas mysql-connector-python jupyter
```

---

### 4. Create MySQL Database

```sql
CREATE DATABASE ecommerce_db;
```

---

### 5. Configure Database Connection

Open `csv_to_sql.py` and update credentials:

```python
conn = mysql.connector.connect(
    host='your_host',
    user='your_username',
    password='your_password',
    database='your_database'
)
```

Also update dataset folder path:

```python
folder_path = 'path_to_your_folder'
```

---

### 6. Load Data into MySQL

```bash
python csv_to_sql.py
```

This automatically creates tables and inserts data.

---

### 7. Run SQL Analysis Notebook

```bash
jupyter notebook
```

Open:

```
python+sql_ecommerce.ipynb
```

Run all cells to perform analysis.

---

## 📈 SQL Analysis Covered

### ✅ Basic Queries
- List unique customer cities
- Count orders placed in 2017
- Total sales per category
- Percentage of installment payments
- Customer count by state

### ✅ Intermediate Queries
- Monthly orders in 2018
- Average products per order by city
- Revenue contribution by category
- Price vs purchase correlation
- Seller revenue ranking

### ✅ Advanced Queries
- Moving average of order values
- Monthly cumulative sales
- Year-over-year sales growth
- Customer retention rate
- Top spending customers per year

---

## 💡 Skills Demonstrated

- SQL Data Analysis
- ETL Pipeline Development
- Database Design
- Data Cleaning
- Analytical SQL
- Business Problem Solving
- Data Engineering Fundamentals

---

## 📊 Real-World Use Cases

- Sales Analytics
- Customer Behavior Analysis
- Revenue Reporting
- Business Intelligence Analytics
- Operational Reporting

---

## 🔮 Future Improvements

- Power BI / Tableau Dashboard
- Cloud Deployment (AWS / Azure)
- Automated ETL Pipelines
- Data Validation Framework
- Interactive Analytics Dashboard

---

## 👩‍💻 Author

**Lahari Prathapagiri**

Email: plahari.prathapagiri94@gmail.com  
GitHub: https://github.com/Lahari-1097  
LinkedIn: https://www.linkedin.com/in/lahari-prathapagiri/

---

⭐ If you found this project useful, consider giving the repository a star!
