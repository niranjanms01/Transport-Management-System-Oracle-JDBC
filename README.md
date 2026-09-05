Transport Management System -- Oracle JDBC
A Java Swing-based Transport Management System developed using Java, JDBC, and Oracle Database. The project demonstrates database design, Oracle connectivity, and CRUD (Create, Read, Update, Delete) operations through a graphical user interface.
📌 Project Overview
The Transport Management System is a DBMS application designed to manage transport-related information such as vehicles, drivers, routes, customers, bookings, and payments.
✨ Features
Vehicle management
Create, Read, Update, and Delete (CRUD) operations
Oracle Database connectivity using JDBC
Relational database design with primary and foreign keys
Java Swing-based graphical user interface
🛠️ Technologies Used
Technology               Purpose
Java                     Application development Java Swing               Graphical user interface JDBC                     Java-to-Oracle connectivity Oracle Database XE 21c   Backend database Apache NetBeans          Development environment Docker                   Running Oracle Database locally
🗄️ Database Design
The database contains:
VEHICLES
DRIVERS
ROUTES
CUSTOMERS
BOOKINGS
PAYMENTS
Relationships
CUSTOMERS ───────┐
                 │
VEHICLES ────────┼──> BOOKINGS ───> PAYMENTS
                 │
ROUTES ──────────┘
🔗 Oracle Database Connection
The application uses JDBC to connect to Oracle Database.
Host: localhost
Port: 1521
Service Name: XEPDB1
Username: system
JDBC URL: jdbc:oracle:thin:@localhost:1521/XEPDB1
Security: Do not upload your actual Oracle database password to GitHub. Configure it locally.
🐳 Running Oracle with Docker
Example command:
docker run -d --name oracle-xe -p 1521:1521 -e ORACLE_PASSWORD=YOUR_PASSWORD gvenzl/oracle-xe
Check the container:
docker ps
📂 Project Structure
Transport-Management-System-Oracle-JDBC/
│
├── src/
│   └── transportmanagementsystem/
│       ├── TransportManagementSystem.java
│       ├── VehicleForm.java
│       └── VehicleForm.form
│
├── database/
│   ├── schema.sql
│   └── sample_data.sql
│
├── lib/
│   └── ojdbc8.jar
│
├── screenshots/
│
├── README.md
└── report.pdf
⚙️ Setup
Install a compatible Java JDK.
Install Apache NetBeans.
Open the project in NetBeans.
Add the Oracle JDBC driver (ojdbc8.jar) to the project Libraries.
Start the Oracle XE Docker container.
Open Oracle SQL Developer.
Execute database/schema.sql.
Configure the JDBC connection details in the Java application.
Run VehicleForm.java from NetBeans.
🔄 CRUD Operations
Create
Adds a new vehicle record to the Oracle database.
Read
Retrieves vehicle records from the database.
Update
Modifies an existing vehicle record.
Delete
Removes a vehicle record from the database.
📸 Screenshots
Place application screenshots inside the screenshots folder.
Example:
![Vehicle Management GUI](screenshots/vehicle-form.png)
🎓 Academic Project
This project demonstrates:
Relational database design
Primary and foreign keys
CRUD operations
JDBC integration
Java Swing GUI development
End-to-end database application functionality
🚀 Future Enhancements
CRUD interfaces for all database tables
Search and filtering
User authentication
Booking management
Payment management
Dashboard and reports
Improved input validation
👨‍💻 Author
Niranjan M S
Transport Management System -- Java + Oracle JDBC
