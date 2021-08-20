1. Environment Preparation
a. OS recommendation:
Ubuntu Linux 18.04
b. Application Server:
Download and install Django 2.1.5
c. Database Server:
Download and install MySQL 5.7
Note: table names are not case-sensitive.
d. Connection Pool
Download and install DBUtils 1.3


2.Database initialization
a. Create a database named ***, e.g. training.
b. Under MySQL client, enter into the *** to run db/sys_setup.sql 

3. Application Deployment
a. Copy src to Django installation directory. If src has already exist, delete it first.
b. Modify Connection Pool configuration:
    Inside src/trydjango/settings.py, from lines 88-103, change DATABASES by replacing NAME with your MySQL database name ***, USER with your MySQL account username, PASSWORD with your MySQL database password. Keep everything else unchanged.
    Inside src/training/db.py, from lines 7-24, change POOL by replacing database with your MySQL database name ***, user with your MySQL account username, password with your MySQL database password. Keep everything else unchanged.


4. Run Django

5. Open browser and visit URL: http://127.0.0.1:8000

See project.info for more details

