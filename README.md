# Kapture_CRM_call

Call Analytics
Call Analytics is a Java program that analyzes call data stored in a MySQL database and provides insights such as the hour of the day with the highest call volume, the hour of the day with the longest calls, the day of the week with the highest call volume, and the day of the week with the longest calls.

Requirements
Java Development Kit (JDK) 8 or later
MySQL database server
MySQL Connector/J JDBC driver
Installation
Clone or download the Call Analytics source code from GitHub.
Install the JDK if it is not already installed on your system.
Install the MySQL database server if it is not already installed on your system.
Install the MySQL Connector/J JDBC driver. You can download the driver from the MySQL website: https://dev.mysql.com/downloads/connector/j/
Create a new MySQL database and table to store the call data. You can use the following SQL commands to create the table:
sql
Copy code
CREATE DATABASE database_db;
USE database_db;

CREATE TABLE call_ana (
  id INT(11) NOT NULL AUTO_INCREMENT,
  from_number VARCHAR(255) NOT NULL,
  start_time DATETIME NOT NULL,
  end_time DATETIME NOT NULL,
  duration INT(11) NOT NULL,
  PRIMARY KEY (id)
);
Update the DB_URL, USER, and PASS constants in the CallAnalytics class to match your MySQL database configuration.
Compile the Call Analytics program using the following command:
Copy code
javac CallAnalytics.java
Usage
To run the Call Analytics program, use the following command:

Copy code
java CallAnalytics
The program will output the following information:

The hour of the day with the highest call volume
The hour of the day with the longest calls
The day of the week with the highest call volume
The day of the week with the longest calls
