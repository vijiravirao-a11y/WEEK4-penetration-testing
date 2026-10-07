# WEEK 4 – DATABASE BACKUP ANALYSIS

## 📌 Project Overview

In Week 4 of my cybersecurity learning journey, I worked on **analyzing an SQL database backup** using Kali Linux.

The main focus of this activity was to understand how database backup files are structured, search for specific tables and information, and identify the type of data stored inside the backup.

I used Linux command-line tools such as `grep` to search through the SQL backup file and locate the required database information.

---

## 🎯 Objective

The main objectives of this week's activity were:

* To understand the structure of an SQL database backup.
* To practice searching large SQL files using Linux commands.
* To identify specific database tables.
* To examine the structure and stored records of a table.
* To understand how sensitive information can be exposed through unsecured database backups.
* To improve practical Linux and cybersecurity investigation skills.

---

## 🛠️ Tools Used

* **Kali Linux**
* **Linux Terminal**
* **Grep**
* **SQL Database Backup File**

---

## 🔍 Work Performed

### 1. Obtained the Database Backup

I worked with an old SQL database backup file named:

`mediroza_db_backup_2019.sql`

The file contained database-related information, including table structures and stored data.

---

### 2. Searched the SQL Backup

I used the Linux `grep` command to search for information related to the `staff` table.

Example command:

```bash
grep -ni "staff" mediroza_db_backup_2019.sql
```

This helped me locate different sections of the SQL file where the word `staff` appeared.

---

### 3. Identified the Staff Table

From the search results, I identified sections related to the `staff` table.

The output contained information such as:

* Warning messages
* Table structure
* `DROP TABLE IF EXISTS staff`
* `CREATE TABLE staff`
* Data dumping information

This helped me understand how a database table is represented inside an SQL backup file.

---

### 4. Examined the Table Structure

The `CREATE TABLE staff` section showed the fields/columns used by the table.

The staff table contained fields related to employee information, such as:

* ID
* Full name
* Job title
* Department
* Email
* Phone
* National ID
* Salary
* Date joined

This demonstrated how structured information is stored inside a relational database.

---

### 5. Located the Stored Records

I then examined the data associated with the `staff` table.

The backup contained **10 staff records**.

These records demonstrated that database backups may contain a large amount of sensitive information in a readable format.

For cybersecurity documentation, the actual personal information was not included publicly.

---

## 💻 Linux Command Used

The main command used during the analysis was:

```bash
grep -ni "staff" mediroza_db_backup_2019.sql
```

### Meaning of the command

* `grep` → Searches for specific text inside a file.
* `-n` → Displays the line number where the matching text is found.
* `-i` → Makes the search case-insensitive.
* `"staff"` → The text being searched for.
* `mediroza_db_backup_2019.sql` → The SQL backup file being searched.

This command was useful for quickly locating relevant sections inside a large SQL file.

---

## 📊 Findings

During the analysis, I identified:

* The `staff` database table.
* The table structure.
* The columns associated with the table.
* The stored staff records.
* 10 records available in the backup.
* Sensitive information stored within the database.

The activity showed how much information can potentially be exposed when a database backup is not properly protected.

---

## 🔐 Security Awareness

Database backups can contain sensitive information such as:

* Personal details
* Contact information
* Employee information
* Identification information
* Salary-related information

Therefore, database backups should be:

* Properly secured.
* Access-controlled.
* Encrypted when appropriate.
* Stored in protected locations.
* Prevented from being publicly accessible.
* Handled carefully during testing and investigation.

Sensitive information discovered during this activity should **not be published in screenshots or GitHub files**.

---

## 🧠 What I Learned

Through this activity, I learned:

* How SQL database backups are structured.
* How to search large files using `grep`.
* How to identify database tables inside an SQL dump.
* How `CREATE TABLE` and data-dumping sections appear in a backup.
* How database backups can expose sensitive information.
* The importance of protecting backup files.
* The importance of responsible handling of sensitive data during cybersecurity investigations.

---

## 📸 Evidence

The project contains screenshots showing the practical work performed during the activity.

The screenshots should include:

1. SQL backup file in Kali Linux.
2. Terminal showing the `grep` search.
3. Search results identifying the `staff` table.
4. Relevant database structure/output.

**Sensitive personal information has been blurred, hidden, or excluded from public screenshots.**

---

## ⚠️ Disclaimer

This activity was performed for **educational and cybersecurity learning purposes**.

The database was analyzed only to understand SQL backup structures, information discovery, and database security concepts.

No attempt was made to misuse, modify, or distribute the sensitive information contained in the backup.

---

## 📚 Skills Practiced

* Linux command line
* `grep`
* SQL database analysis
* SQL dump analysis
* Database structure identification
* Information discovery
* Sensitive data awareness
* Basic database security
* Cybersecurity investigation

---

## 📅 Week 4 Summary

**Week:** 4
**Project:** Database Backup Analysis
**Focus:** SQL Dump Analysis & Information Discovery
**Platform:** Kali Linux
**Primary Tool:** Linux Terminal / `grep`

This week's activity gave me practical experience in examining a database backup and understanding how sensitive information can be exposed if database backups are not properly secured.

It also improved my confidence in using Linux commands for cybersecurity investigation and information discovery.

---

## 👤 Author

**Vijayalakshmi Bai**
Cybersecurity Learner
