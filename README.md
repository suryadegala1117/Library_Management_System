# Library Management System
## Overview
The Library Management System is a Python application built using the Tkinter library for the graphical user interface and pymysql for database connectivity. It serves as a tool for managing a library's inventory and tracking book issuances.

## Features
### Librarian Interface:

Add books to the library database.
Issue and return books to/from students.
View available books.
View books that have been issued.
Delete books from the database.
### Admin Interface:
Add and manage users (librarians or other admins).
View user information.
Delete users.
### Prerequisites
Before running the application, ensure you have Python installed on your system. Additionally, you need to install the pymysql package for MySQL database connectivity:
    <pre><code> pip install pymysql
    </code></pre>
### Usage
**1.** Clone or download this repository.

**2.** Navigate to the project directory:
    <pre><code>cd Library-Management-System
    </code></pre>
### Run The Appliaction
<pre><code>python library_management_system.py
</code></pre>
**1.** Log in as a librarian or an admin.
**2.** For librarians, you can manage books, issue/return books, etc.
**3.** Admins can add/manage users.
### Database Setup
The application uses a MySQL database to store book and user information. You need to set up a MySQL server and create the necessary database and tables. Here are the steps:

**1.** Install MySQL on your system if it's not already installed.

**2.** Start the MySQL server.

**3.** Create a new database named "Library."

**4.** Create the following tables within the "Library" database:

     Book: To store book information (subject, title, author, serial number).
     BookIssue: To track book issuance (student ID, serial number, issue date, expiry date).
     Login: To store user information (name, user ID, branch, mobile number).
    
**5.** Update the database connection details in the code (library_management_system.py) to match your MySQL server configuration:
<pre><code>con = p.connect(host="localhost", user="root", password="your_mysql_password", database="Library")
</code></pre>
### Contributing
Contributions are welcome! If you find any bugs, want to add new features, or have suggestions for improvements, please feel free to open an issue or submit a pull request.



