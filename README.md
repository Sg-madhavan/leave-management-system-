# Leave Management System

A web-based Leave Management System developed using **Python Flask REST API and MySQL** to simplify employee leave applications, tracking, and management.

## 🚀 Project Overview

The Leave Management System allows employees to apply for leave, view their leave records, update leave requests, and track their application status.

The application uses Flask REST APIs for backend operations, MySQL for database management, and HTML, CSS, and JavaScript for the frontend.

## 🛠️ Technologies Used

- **Backend:** Python, Flask
- **API Architecture:** REST API
- **Database:** MySQL
- **Frontend:** HTML, CSS, JavaScript
- **Data Exchange:** JSON
- **API Communication:** JavaScript Fetch API

## ✨ Features

- **Leave Application:** Employees can submit leave requests.
- **View Leave Records:** Retrieve and view leave application details.
- **Update Leave Requests:** Modify existing leave request information.
- **Cancel Leave:** Delete or cancel leave applications.
- **Leave Status Management:** Track leave requests with Pending, Approved, and Rejected statuses.
- **RESTful API Integration:** Perform CRUD operations using HTTP methods.
- **Database Integration:** Store and manage employee and leave-related information using MySQL.

## 🔄 CRUD Operations

| Operation | HTTP Method | Description |
|---|---|---|
| Create | POST | Submit a new leave application |
| Read | GET | Retrieve leave application records |
| Update | PUT | Modify existing leave details |
| Delete | DELETE | Cancel or remove a leave application |

## 📂 Project Structure

```text
Leave-Management-System/
│
├── app.py
├── templates/
│   ├── login.html
│   ├── dashboard.html
│   └── ...
│
├── static/
│   ├── css/
│   ├── js/
│   └── images/
│
├── requirements.txt
└── README.md
```

## ⚙️ Installation and Setup

### 1. Clone the Repository

```bash
git clone YOUR_GITHUB_REPOSITORY_LINK
```

### 2. Navigate to the Project Directory

```bash
cd Leave-Management-System
```

### 3. Create a Virtual Environment

```bash
python -m venv .venv
```

### 4. Activate the Virtual Environment

**Windows:**

```bash
.venv\Scripts\activate
```

### 5. Install Dependencies

```bash
pip install flask mysql-connector-python
```

If a `requirements.txt` file is available, use:

```bash
pip install -r requirements.txt
```

### 6. Configure MySQL Database

- Open MySQL Workbench.
- Create the required database.
- Create the necessary tables for employee and leave management.
- Update the database connection credentials in `app.py`.

Example:

```python
def get_db_connection():
    return mysql.connector.connect(
        host="localhost",
        user="root",
        password="YOUR_MYSQL_PASSWORD",
        database="leave_management",
        port=3306
    )
```

**Note:** Replace the database name and credentials with your actual MySQL configuration. Do not upload real database passwords to GitHub.

### 7. Run the Application

```bash
python app.py
```

The Flask development server will start. Open the local application URL displayed in your terminal.

## 📡 REST API Endpoints

The following table describes the intended API operations. Update the endpoint paths to match your actual Flask routes.

| HTTP Method | API Endpoint | Description |
|---|---|---|
| POST | `/api/leaves` | Submit a leave application |
| GET | `/api/leaves` | Retrieve all leave applications |
| GET | `/api/leaves/<id>` | Retrieve a specific leave application |
| PUT | `/api/leaves/<id>` | Update a leave application |
| DELETE | `/api/leaves/<id>` | Delete or cancel a leave application |

## 🔗 Application Architecture

```text
          Frontend
      (HTML, CSS, JS)
              |
              |
       JavaScript Fetch
              |
              |
       Flask REST API
              |
              |
       MySQL Connector
              |
              |
         MySQL Database
```

## 📌 Key Learning Outcomes

- Developed RESTful APIs using Python Flask.
- Implemented CRUD operations using HTTP methods.
- Integrated Flask with MySQL database.
- Understood JSON data exchange between frontend and backend.
- Connected frontend and backend using JavaScript Fetch API.
- Applied relational database concepts for data management.

## 👨‍💻 Author

**Your Name**

- GitHub: YOUR_GITHUB_PROFILE_LINK
