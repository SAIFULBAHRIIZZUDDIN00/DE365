PostgreSQL Installation & Rental DVD Database Setup (Windows)
This guide explains how to install PostgreSQL on Windows and restore the Rental DVD sample database for learning and practice.

1. Download PostgreSQL
Go to the official PostgreSQL website:
👉 https://www.postgresql.org/download/windows/
Download the latest PostgreSQL installer for Windows.

2. Install PostgreSQL
Double-click the downloaded .exe file
Choose the installation directory
(Default location is recommended)
Select components:
✅ PostgreSQL Server
✅ pgAdmin
✅ Command Line Tools

Set a password for the postgres superuser
⚠️ Important: Remember this password

Choose the port
Default: 5432 (recommended)
Complete the installation

3. Prepare Rental DVD Database
Download the rentaldvd.tar file   (https://neon.com/postgresqltutorial/dvdrental.zip)
Extract it if necessary (keep the .tar file)

4. Create Database & Restore Data
Open Command Prompt or PowerShell
Login to PostgreSQL
psql -U postgres


Enter the password when prompted.
Create a new database
CREATE DATABASE rentaldvd;
Restore the database from .tar file
pg_restore -U postgres -d rentaldvd "C:\path\to\rentaldvd.tar"
📌 Replace the path with the actual location of your rentaldvd.tar file.

5. Verify Installation
Login to the restored database:
psql -U postgres -d rentaldvd
Run test commands:
\dt;                     -- List all tables
SELECT COUNT(*) FROM film;  -- Test query
If tables are listed and the query returns a number, the setup is successful ✅

✅ Result
PostgreSQL is installed correctly, and the Rental DVD database is ready for:
SQL practice
Data analysis
Learning joins, subqueries, and indexes
