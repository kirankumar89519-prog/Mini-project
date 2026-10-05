# Bank Account Management System

Student: M KIRAN KUMAR
USN: 1VJ25CI018
Project: Bank Account Management System
Date: 10/05/2026

## Description
A Java console-based Bank Account Management System using MySQL. The application allows bank staff/users to create customer accounts and perform basic banking operations such as deposit, withdrawal, balance enquiry, and transaction record storage.

## Features
1. Create Customer Account
2. View All Accounts
3. Search Account
4. Deposit Money
5. Withdraw Money
6. Balance Enquiry
7. View Transaction History
8. Update Customer Details
9. Close/Delete Account
10. Exit

## Technologies
- Java 17+
- JDBC
- MySQL
- Maven

## Database
Database name: `bank_management`

## Setup
1. Install MySQL and create/use a MySQL user.
2. Open `sql/bank_management.sql` in MySQL Workbench or the MySQL command line and execute it.
3. Open `src/main/java/com/bank/DBConnection.java` and change the MySQL username/password if required.
4. Make sure Maven and Java 17+ are installed.
5. From the project folder, run:
   `mvn compile exec:java`

## Notes
- Account numbers are generated automatically.
- Deposit and withdrawal operations are stored in the `transactions` table.
- Withdrawal is rejected when the requested amount is greater than the available balance.
- Database operations use JDBC PreparedStatements and transactions where required.
