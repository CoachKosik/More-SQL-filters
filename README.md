# More-SQL-filters

## Objective

To gain practical experience in using comparison operators to filter data in SQL queries. By mastering these skills, users can effectively extract relevant information from databases, enabling them to investigate security incidents, analyze trends, and make informed decisions. 

## Project description
This project focuses on using SQL operators to filter data based on numerical and date-time criteria. By leveraging operators like `=`, `<`, `>`, `<>`, `>=`, and `<=`, users can effectively query databases to identify specific data points. This skill is essential for security analysts to investigate incidents, analyze trends, and make informed decisions. The lab provides hands-on experience in applying these operators to real-world scenarios, such as filtering login attempts and identifying system updates.

## Skills Learned

* **Data Filtering:** Effectively using comparison operators like `=`, `>`, `<`, `<>`, `>=`, and `<=` to filter data based on specific criteria.
* **Date and Time Filtering:** Filtering data based on specific dates and times to identify relevant events.
* **SQL Query Construction:** Building complex SQL queries to extract specific information from a database.
* **Data Analysis:** Interpreting query results to identify potential security threats or anomalies. 

## Tools Used

* **SQL Database:** A database management system used to store and manage structured data.
* **SQL Query Language:** Used to interact with the database and retrieve specific information.
* **MariaDB Shell:** A command-line interface for interacting with the MariaDB database.

## Steps
1. Retrieve login attempts after a certain date
* In this task, you need to investigate a recent security incident. To do this, you need to gather information about login attempts made after a certain date.
  * Complete the SQL query to retrieve data for login attempts made after '2022-05-09'. Replace X with the correct operator:
     * ![more sql 2](https://github.com/user-attachments/assets/c2ad16d7-f660-4235-986b-d63782d4be95)
     * ![more sql 1](https://github.com/user-attachments/assets/6a20c104-dbf3-499e-bc3b-a7d2a78a5745)
  * Now, based on your first query, you find a need to expand the date range to include 2022-05-09 in your search.
     * Complete the SQL query to retrieve data for login attempts that were made on or after '2022-05-09'. Replace X with the correct operator:
     * ![more sql 3](https://github.com/user-attachments/assets/3dc70a90-de92-46c7-807a-84429c3a9939)
     * ![image](https://github.com/user-attachments/assets/9ac6f57e-1449-44cc-91fe-478fae7c9eb4)
      
2. Retrieve logins in a date range
* In this task, you need to narrow the focus of the search. Login attempts made after 2022-05-11 shouldn't be included. Use the BETWEEN and AND operators to return results between '2022-05-09' and '2022-05-11'.
  * Run the query to retrieve the required records. You must insert the required dates X and Y:
    * ![more sql 5](https://github.com/user-attachments/assets/6ed868d4-04f7-4edc-98c9-fdddcb22e132)
    * ![more sql 6](https://github.com/user-attachments/assets/f8e84e01-7e72-45db-9362-cbf3be134a5d)

3. Investigate logins at certain times
* In this task, you need to investigate logins that were made at certain times. To do this, filter the data in the log_in_attempts table by login time (login_time).
  * First, your organization's typical work hours begin at 07:00:00. Retrieve all login attempts made before 07:00:00 to learn more about the users who are logging in outside of typical hours.
    * Write a SQL query to retrieve data for login attempts made before '07:00:00'.
    * ![image](https://github.com/user-attachments/assets/5e51e318-d776-46e2-8cf1-b03f5cb7e37f)
  * The query in the previous step returned more results than required.
    * Modify the query to return logins between '06:00:00' and '07:00:00'.
    * ![image](https://github.com/user-attachments/assets/9dd8b6c0-f98c-46a8-8274-be8aed4dac63)

4. Investigate logins by event ID
* In this task, you need to investigate login attempts based on event ID numbers. With this query, you want to return only the event_id, username, and login_date fields from the log_in_attempts table.
  * Write a query to return login attempts with event_id greater than or equal to 100.
    * ![more sql 9](https://github.com/user-attachments/assets/8079a129-cecd-47f9-8d1f-dd978242ca8b)
  * The query in the previous step returned more data than required.
    * Modify the query to return only login attempts with event_id between 100 and 150.
    * ![more sql 10](https://github.com/user-attachments/assets/911178af-cbae-48dc-a0ac-68ed21466e80)

### Summary

This activity provided hands-on experience in filtering data from a database using SQL. By employing WHERE clauses, BETWEEN and AND operators, and comparison operators, users can effectively extract specific subsets of data, enabling deeper analysis and informed decision-making.
