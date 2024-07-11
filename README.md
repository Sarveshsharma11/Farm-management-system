# Farm Management System

## Overview

This project is designed for agricultural purposes where farmers can keep track of their agro products. It provides an intuitive interface for managing various aspects of farming, including authentication, registration, CRUD operations, and selling products.

## Features

1. **Authentication System**: Secure login and registration for farmers.
2. **Farmers Registration**: Registration system for new farmers.
3. **CRUD Operations**: Create, read, update, and delete operations for managing records.
4. **Seeds-wise Records**: Maintain records based on different types of seeds.
5. **Adding Agro Products**: Farmers can add new agro products to the system.
6. **Triggers**: Automated actions based on specific events.
7. **View Records**: Farmers can view their records.
8. **Sell Agro Products**: Farmers can list their products for sale.



## Requirements

To run this project, you need the following Python modules:

- Flask
- Flask-SQLAlchemy
- mysqlclient
- Flask-Login

Install the required modules using the following commands:

```sh
pip install flask
pip install Flask-SQLAlchemy
pip install mysqlclient
pip install Flask-Login
```

## How to Run the Project

### Step 1: Clone the Repository

First, clone the repository to your local machine using Git:

```sh
git clone https://github.com/yourusername/farm-management-system.git
```

### Step 2: Navigate to the Project Directory

Change your working directory to the project folder:

```sh
cd farm-management-system
```

### Step 3: Set Up the Database

Make sure you have MySQL installed and running. Create a database for the project:

```sql
CREATE DATABASE farm_management;
```

Update the database configuration in your project to connect to your MySQL database. Typically, this will be in a configuration file or within your Flask app setup:

```python
app.config['SQLALCHEMY_DATABASE_URI'] = 'mysql://username:password@localhost/farm_management'
```

Replace `username` and `password` with your MySQL credentials.

### Step 4: Initialize the Database

Run the following commands to set up the database schema:

```sh
from your_project_name import db
db.create_all()
```

### Step 5: Run the Application

Finally, start the Flask application:

```sh
python app.py
```

Your application should now be running on `http://127.0.0.1:5000/`.


