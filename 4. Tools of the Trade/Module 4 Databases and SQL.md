# Introduction to SQL and Databases

## Introduction to databases

This session dives into the fundamental concepts of databases, emphasizing their importance for security analysts and how relational databases are structured.

- **Databases: The Cornerstone of Data Storage and Management**
    
    - Databases are organized collections of structured information, often compared to spreadsheets.
    - They excel at storing massive amounts of data, enabling simultaneous access by multiple users, and facilitating complex data retrieval tasks.
    - Security analysts frequently interact with databases containing critical security-related information, such as login attempts, software updates, and machine ownership details.
    
- **Relational Databases: A Structured Approach**
    
    - Relational databases are a type of database that structures data into interconnected tables.
    - Each table focuses on a specific entity (e.g., employees) and contains columns (fields) that define the characteristics of that entity (e.g., employee_id, device_id, username).
    - Rows (records) represent individual instances within a table. Each row contains data points corresponding to the columns (e.g., a record for an employee with ID 1000 working in marketing).
    
- **Connecting the Dots: Keys and Relationships in Relational Databases**
    
    - Relational databases establish connections between tables using columns they share in common.
        
    - These shared columns are called keys.
        
    - **Primary Key:**
        
        - A unique identifier for each row within a table.
        - Enforces uniqueness (no duplicates) and ensures no missing values (null or empty).
        - Example: The employee_id in the employee table; each employee has a unique ID.
        
    - **Foreign Key:**
        
        - A column in one table that references the primary key of another table.
        - Allows for linking related data between tables.
        - Can have duplicates and null values, unlike primary keys.
        - Example: The employee_id column in the machines table; it connects each machine to its assigned employee using the employee_id from the employee table (the primary key).
        
    - **Key Points:**
        
        - A table can only have one primary key but can have multiple foreign keys.
        - Understanding these key relationships is essential for working effectively with relational databases.
        
    
- **Moving Forward: Exploring SQL**
    
    - SQL (Structured Query Language) is the language used to interact with relational databases.
    - In the following sections, you'll gain hands-on experience working with the database concepts covered in this session.

## Query databases with SQL

This session highlights the significance of SQL (Structured Query Language) for security analysts, exploring how it empowers them to interact with databases and extract valuable insights.

- **SQL: The Bridge Between Security Analysts and Databases**
    
    - As a security analyst, proficiency in accessing and querying databases is essential.
    - SQL serves as the bridge between you and the data, allowing you to:
        
        - Create databases.
        - Interact with existing databases.
        - Request specific information from databases.
        
    
- **Understanding Queries: The Heart of Data Retrieval**
    
    - A query acts as a specific request for data from a database table (or a combination of tables).
    - Relational databases heavily rely on SQL variations for querying data.
    - While minor syntax differences exist between SQL versions (e.g., quotation mark placement), the core functionality remains consistent.
    - Mastering SQL equips you with a powerful toolset for effective security analysis tasks.
    
- **Leveraging SQL for Log Analysis**
    
    - Security analysts heavily rely on logs, which record events within an organization's systems.
        
    - SQL empowers you to efficiently analyse these logs for various purposes:
        
        - Identifying misconfigured machines by filtering logs containing machine details.
        - Detecting suspicious activity on websites or web applications by searching for unusual visitor patterns in relevant logs.
        
    - **The Power of Efficiency:** Security logs can be massive, making manual inspection daunting. SQL simplifies this process by enabling you to:
        
        - Search through millions of data points.
        - Extract relevant information using targeted queries that run in seconds.
        
    
- **Beyond Log Analysis: SQL for Basic Data Analytics**
    
    - SQL's capabilities extend beyond log analysis, providing a foundation for basic data analytics, another valuable skill for security analysts.
    - Utilize SQL filtering to pinpoint data that informs security decisions and helps anticipate potential issues.
        
        - Example 1: Identify machines lacking the latest security patches, crucial for maintaining system protection.
        - Example 2: Determine optimal times for system updates based on low-usage periods, minimizing disruption.
        
    
- **Moving Forward: Hands-on Practice with SQL**
    
    - With a solid understanding of SQL's importance, you're prepared to delve into crafting your own basic queries using a sample database in the next video!

## SQL filtering versus Linux filtering

This guide equips you, as a security analyst, to distinguish between SQL and Linux filtering techniques, highlighting their strengths and ideal use cases.

- **Understanding the Filtering Landscape**
    
    - You've previously explored filtering data using both Linux commands and SQL.
    - This session delves into the key differences between these two approaches to empower you to make informed choices when filtering data for security analysis.
    - Additionally, you'll discover that you can access SQL functionalities through the Linux command line.
    
- **Accessing SQL Through Linux**
    
    - Numerous interfaces and variations of SQL exist.
    - The Linux command line provides one access point to SQL.
    - To initiate an SQL session using Linux, enter the specific command for your desired SQL version. For instance, use `sqlite3` to access SQLite.
    - Subsequent commands will be directed to SQL instead of the standard Linux shell commands.
    
- **Distinguishing Between Linux and SQL Filtering**
    
    - While both Linux and SQL facilitate data filtering, their purposes and functionalities differ significantly.
        
        - **Purpose:**
            
            - **Linux:** Filters data within the context of a computer system's files and directories. Common tasks include searching for specific files, managing file permissions, and handling processes.
            - **SQL:** Designed for filtering data stored within a database management system. It empowers you to query and manipulate data organized in tables, retrieving specific information based on defined criteria.
            
        - **Syntax:**
            
            - **Linux:** Employs various commands and command-line options specific to each filtering tool. The syntax varies depending on the tool's purpose. Examples include `find`, `sed`, `cut`, and `grep`.
            - **SQL:** Leverages Structured Query Language (SQL), a standardized language featuring specific keywords and clauses for filtering data across diverse SQL databases. Examples include keywords like `WHERE` and `SELECT`, and clauses like `JOIN`.
            
        - **Structure:**
            
            - **Linux:** Offers a more free-form, less structured approach.
            - **SQL:** Provides a significantly more structured environment. For instance, when examining employee login attempt logs, SQL presents each record separated into distinct columns. In contrast, Linux would display the data as a single line of unformatted text. This structured organization in SQL allows for easier and more efficient selection of specific columns for analysis.
            - SQL yields results that are inherently more readable and adaptable compared to Linux output.
            
        - **Joining Tables:**
            
            - Security-related decisions often necessitate analysing information from multiple tables. SQL grants analysts the ability to join various tables when retrieving data. Linux lacks this functionality, hindering the connection of data points across your computer system, making security log analysis more restrictive.
            
        
    
- **Deciding Between the Tools**
    
    - As a security analyst, proficiency in selecting the appropriate tool for the task is crucial. While SQL offers a structured environment and table joining capabilities, Linux filtering remains valuable in specific scenarios.
    - Security-related data is often stored in database formats compatible with SQL. However, some logs may exist in non-SQL-compatible formats, such as plain text files. In such cases, Linux filtering expertise becomes essential.
    
- **Key Takeaways**
    
    - Linux filtering excels at managing a system's files and directories, while SQL focuses on structured data manipulation within databases.
    - Leverage the Linux command line as one of several methods to access SQL.
    - Both SQL and Linux provide data filtering functionalities; however, SQL offers advantages in data structuring and facilitating joins between multiple tables.
---
# SQL queries

## Basic queries

This session dives into practical SQL application by guiding you through your very first SQL query, a task commonly encountered by security analysts.

- **Introduction: Your First SQL Query Awaits**
    
    - This video equips you with the skills to construct and execute your initial SQL query, a fundamental skill for security analysts.
    - The chosen scenario involves pinpointing which computer is assigned to a particular employee.
    
- **The Building Blocks of Basic SQL Queries**
    
    - We'll focus on two essential SQL keywords that lay the foundation for crafting basic SQL queries:
        
        - **SELECT:** This keyword specifies the columns you intend to retrieve from a database table.
        - **FROM:** This keyword identifies the table from which you'll be extracting data.
        
    - The usage of these keywords closely resembles their application in everyday language. For instance, requesting a friend to "select apples and bananas from the big box" at the grocery store mirrors an SQL query structure.
    
- **Constructing Your First Query**
    
    - Let's leverage the `SELECT` and `FROM` keywords to retrieve the necessary employee and computer data:
        
        2. **SQL statement:** Begin by typing the SQL statement.
        4. **FROM clause:** Specify the table from which data will be drawn (e.g., `FROM employees` in this case).
        6. **SELECT clause:** Indicate the columns you want returned from the table using commas to separate them (e.g., `SELECT employee_id, device_id`).
        
    
- **Understanding SQL Syntax**
    
    - **Case Sensitivity:** SQL keywords are not case-sensitive. You can write them in uppercase (e.g., `SELECT`, `FROM`) or lowercase (e.g., `select`, `from`), but using uppercase generally enhances readability.
    - **Semicolons:** SQL statements typically conclude with a semicolon (`;`).
    
- **Executing Your Query and Viewing the Results**
    
    - Run the query by pressing Enter. The output should display the data that links employees to their assigned computers, marking the successful execution of your first SQL query!
    
- **Expanding Your Queries**
    
    - Suppose you require additional information, such as the department, username, or office location for the employee using a specific computer.
    - Utilize SQL to construct a new query that retrieves all columns from the table. Employ the asterisk (*) after `SELECT`, signifying "select all."
    - Execute this new query on the `employees` table to view the entire table in the output.

## Demystifying Your First SQL Queries: A Guided Exploration

This guide revisits fundamental SQL queries and introduces the `ORDER BY` keyword for organizing your retrieved data. It also familiarizes you with the Chinook database, a sample database used throughout this course.

- **Reviewing Basic SQL Queries**
    
    - Recall that two essential keywords form the core of any SQL query:
        
        - **SELECT:** Specifying the columns you intend to retrieve from a database table.
        - **FROM:** Identifying the table from which you'll be extracting data.
    - We previously explored a sample query that retrieves `employee_id` and `device_id` columns from the `employees` table:
        
        ```SQL
        SELECT employee_id, device_id
        FROM employees;
        ```
        
- **Introducing the Chinook Database**
    
    - This course leverages a sample database called Chinook to demonstrate queries in readings and quizzes.
    - Chinook simulates a digital media company's database structure, potentially containing data relevant to a security analyst working for that company.
    - The database encompasses eleven tables, including `employees`, `customers`, and `invoices`, storing information like names and addresses.
- **Crafting Basic SELECT Statements**
    
    - The `SELECT` keyword dictates which columns to return from a table.
        
        - Example 1: Retrieving the `customerid` column:
            
            ```SQL
            SELECT customerid
            FROM customers;
            ```
            
        - Example 2: Selecting both `customerid` and `city` columns:
            
            ```SQL
            SELECT customerid, city
            FROM customers;
            ```
            
    - Utilize the asterisk (*) after `SELECT` to return all columns from a table.
        
        ```SQL
        SELECT *
        FROM customers;
        ```
        
    - **Important Note:** While querying relatively small tables like those in this course, using `SELECT *` might be acceptable. However, this practice is generally discouraged for extensive databases and tables due to potential readability issues and slower execution times.
        
- **The FROM Clause: Specifying the Target Table**
    
    - The `SELECT` keyword invariably accompanies the `FROM` keyword.
        
    - `FROM` indicates the table you intend to query.
        
    - Following the `SELECT` keyword (often on a new line), use `FROM` followed by the name of the table you're querying.
        
        ```SQL
        SELECT *
        FROM customers;
        ```
        
    - Semicolons (;) typically mark the end of an SQL query, signifying completion.
        
    - **Note:** Line breaks aren't mandatory in SQL queries but are commonly used to enhance readability. You can write the previous query on a single line as well:
        
        ```SQL
        SELECT * FROM customers;
        ```
        
- **Organizing Your Output with ORDER BY**
    
    - Database tables can become intricate, necessitating additional SQL keywords for efficient data management.
    - The `ORDER BY` keyword plays a crucial role in organizing the data retrieved from a table.
    - `ORDER BY` sequences the records returned by a query based on a designated column or columns, allowing for either ascending or descending order.
- **Sorting in Ascending Order (Default)**
    
    - To implement `ORDER BY`, add it at the query's end and specify the column for sorting. Here, the query returns `customerid`, `city`, and `country` columns from `customers`, ordered by the `city` column:
        
        ```SQL
        SELECT customerid, city, country
        FROM customers
        ORDER BY city;
        ```
        
    - The `ORDER BY` keyword sorts records based on the column specified after it. By default (as shown in this example), the order will be ascending. This signifies:
        
        - For numeric data columns, sorting occurs from smallest to largest values (e.g., `customerid` sorting IDs from smallest to largest).
        - For alphabetic character columns (like the `city` example), sorting progresses from the beginning of the alphabet to the end.
- **Descending Order with ORDER BY DESC**
    
    - Include `DESC` with `ORDER BY` to sort in descending order. `DESC` stands for "descending" and instructs SQL to sort numbers from largest to smallest or letters alphabetically from Z to A.
        
        ```SQL
        SELECT customerid, city, country
        FROM customers
        ORDER BY city DESC;
        ```
        
    - In this instance, cities with names towards the end of the alphabet will be listed first.
        
- **Sorting Based on Multiple Columns**
    
    - You can designate numerous columns for sorting. For instance, you might prioritize `country` first, followed by `city`. SQL would then sort the output by `country`, and for rows with the same `country`, it would sort them based on `city`.
        ```SQL
        SELECT customerid, city, country
        FROM customers
        ORDER BY country, city;
        ```

- **Key takeaways**

SELECT and FROM are important keywords in SQL queries. You use SELECT to indicate which columns to return and FROM to indicate which table to query. You can also include ORDER BY in your query to organize the output. These foundational SQL skills will support you as you move into more advanced queries.

## Basic filters on SQL queries

This guide equips you with SQL's filtering capabilities, empowering you to extract specific data from databases, a crucial skill for security analysts.

- **The Power of Filtering in SQL**
    
    - This session delves into SQL's filtering functionality, enabling you to make your database queries more precise and retrieve only the information you require.
    
- **Filtering Explained: Selecting Specific Data**
    
    - Filtering refers to the process of selecting data that aligns with certain criteria. Imagine it as a way to sift through a vast amount of data and choose only the relevant pieces.
        
        - Analogy: Selecting apples at a fruit stand – you might choose "only fresh apples," filtering out any that aren't fresh.
        
    - Security analysts leverage filtering to examine specific sets of data within tables. For instance, filtering a login attempts table to identify all attempts originating from a particular country.
    
- **Operators: The Building Blocks of Filtering**
    
    - Operators are symbols or keywords representing operations within an SQL statement.
        
        - Example: The equal to sign (`=`) is an operator.
        
    - To filter an SQL query, you add a `WHERE` clause that specifies the filtering condition using operators.
        
        - Example: Finding login attempts from the United States:
            
            ```SQL
            WHERE country = 'USA'
            ```
            
        
    
- **Constructing Your First Filter**
    
    - Let's build a query that retrieves all columns from the `log_in_attempts` table and filters the results to include only entries where the `country` is "USA":
        
        ```SQL
        SELECT *
        FROM log_in_attempts
        WHERE country = 'USA';
        ```
        
    
- **Filtering Beyond Exact Matches: Using Patterns**
    
    - Our previous example used a filter based on an exact value ("USA"). We can create more intricate filters by searching for patterns instead of precise terms.
        
        - Example: Finding offices in the East building within an `employees` table:
            
            - The percent sign (%) acts as a wildcard for unspecified characters.
            - A filter for `'East%'` would return entries like "East-120," "East-290," and "East-435."
            
        
    
- **LIKE: The Operator for Pattern Matching**
    
    - When searching for patterns using the percent sign, we don't use the equal to sign (`=`). Instead, we employ the `LIKE` operator within the `WHERE` clause.
        
        - Example: Retrieving entries from the `office` column that begin with "East":
            
            ```SQL
            WHERE office LIKE 'East%'
            ```
            
        
    
- **LIKE in Action: Handling Inconsistencies**
    
    - Imagine our database has inconsistencies in how the United States is represented ("US" vs. "USA").
    - We can leverage `LIKE` to filter for entries containing "US" at the beginning:
        
        ```SQL
        WHERE country LIKE 'US%'
        ```
        
    - This captures entries with both "US" and "USA."
    
- **Conclusion: Precise Data Retrieval**
    
    - By effectively using SQL filtering techniques, you've gained the ability to construct highly targeted database queries, retrieving only the exact data you require. This empowers you to conduct in-depth analyses as a security analyst.

- **The WHERE clause and basic operators**

Previously, you focused on how to refine your SQL queries by using the WHERE clause to filter results. In this reading, you’ll further explore how to use the WHERE clause, the LIKE operator and the percentage sign (%) wildcard. You’ll also be introduced to the underscore (_), another wildcard that can help you filter queries.

- **How filtering helps**

As a security analyst, you'll often be responsible for working with very large and complicated security logs. To find the information you need, you'll often need to use SQL to filter the logs.

In a cybersecurity context, you might use filters to find the login attempts of a specific user or all login attempts made at the time of a security issue. As another example, you might filter to find the devices that are running a specific version of an application.

- **WHERE **

To create a filter in SQL, you need to use the keyword WHERE. WHERE indicates the condition for a filter.

If you needed to email employees with a title of IT Staff, you might use a query like the one in the following example. You can run this example to examine what it returns: 


```SQL
SELECT firstname, lastname, title, email

FROM employees

WHERE title = 'IT Staff';
```

Rather than returning all records in the employees table, this WHERE clause instructs SQL to return only those that contain 'IT Staff' in the title column. It uses the equals sign (=) operator to set this condition.

**Note:** You should place the semicolon (;) where the query ends. When you add a filter to a basic query, the semicolon is after the filter. 

- ** Filtering for patterns**

You can also filter based on a pattern. For example, you can identify entries that start or end with a certain character or characters. Filtering for a pattern requires incorporating two more elements into your WHERE clause:

- a wildcard 
    
- the LIKE operator
    

- **Wildcards**

A **wildcard** is a special character that can be substituted with any other character. Two of the most useful wildcards are the percentage sign (%) and the underscore (_):

- The percentage sign substitutes for any number of other characters. 
    
- The underscore symbol only substitutes for one other character.
    

These wildcards can be placed after a string, before a string, or in both locations depending on the pattern you’re filtering for.

The following table includes these wildcards applied to the string 'a' and examples of what each pattern would return.

|**Pattern**|**Results that could be returned**|
|---|---|
|'a%'|apple123, art, a|
|'a_'|as, an, a7|
|'a__'|ant, add, a1c|
|'%a'|pizza, Z6ra, a|
|'_a'|ma, 1a, Ha|
|'%a%'|Again, back, a|
|'_a_'|Car, ban, ea7|

-  **LIKE**

To apply wildcards to the filter, you need to use the LIKE operator instead of an equals sign (=). LIKE is used with WHERE to search for a pattern in a column. 

For instance, if you want to email employees with a title of either 'IT Staff' or 'IT Manager', you can use LIKE operator combined with the % wildcard:  


```SQL
SELECT lastname, firstname, title, email

FROM employees

WHERE title LIKE 'IT%';
```


This query returns all records with values in the title column that start with the pattern of 'IT'. This means both 'IT Staff' and 'IT Manager' are returned.

As another example, if you want to search through the invoices table to find all customers located in states with an abbreviation of 'NY', 'NV', 'NS' or 'NT', you can use the 'N_' pattern on the state column:


```SQL
SELECT firstname,lastname, state, country

FROM customers

WHERE state LIKE 'N_';
```


This returns all the records with state abbreviations that follow this pattern.

- **Key takeaways**

Filters are important when refining what your query returns. WHERE is an essential keyword for adding a filter to your query.  You can also filter for patterns by combining the LIKE operator with the percentage sign (%) and the underscore (_) wildcards.

# More SQL filters
## Filter dates and numbers

This session expands your SQL proficiency by introducing filtering techniques for various data types: strings, numerics, and dates/times. It's crucial for security analysts to effectively query these data types to extract relevant information.

### Common Data Types in Databases

Databases typically store information in three fundamental data types:

2. **String:** An ordered sequence of characters, encompassing letters, numbers, or symbols. Examples include usernames (e.g., "analyst10").
4. **Numeric:** Data consisting of numbers, allowing for mathematical operations like addition or multiplication. Examples include login attempt counts.
6. **Date and Time:** Data representing a specific date and/or time.

### Filtering Beyond String Data

While we previously explored filtering with string data, this session delves into filtering numeric and date/time data, which is often pertinent for security analysts.

- **Use Cases for Security Analysts**
    
    - Filtering patch dates to identify outdated machines requiring updates.
    - Filtering login attempts to pinpoint those occurring within a specific timeframe.
    

### Operators for Numeric and Date/Time Data

We'll leverage operators, introduced in the prior video, to construct filters for numeric and date/time data. Common operators include:

- Equals (`=`)
- Greater Than (`>`)
- Less Than (`<`)
- Not Equal To (`<>`)
- Greater Than or Equal To (`>=`)
- Less Than or Equal To (`<=`)

### Filtering Login Attempts After a Specific Time

Let's illustrate filtering login attempts made after 6 pm, a timeframe potentially indicating suspicious activity.

2. **Crafting the SQL Query:**
    
    - Begin by selecting all columns (`*`) from the `log_in_attempts` table:
        
        ```sql
        SELECT *
        FROM log_in_attempts
        ```
        
    - Add the `WHERE` clause to specify the filtering condition.
    
4. **Filtering Condition:**
    
    - The condition utilizes the `>` (greater than) operator to target entries where the `time` column value is later than '18:00' (representing 6 pm in SQL format).
        
        ```sql
        WHERE time > '18:00'
        ```
        
    
6. **Executing the Query:**
    
    - Run the query to view the results, displaying a list of login attempts occurring after 6 pm.
    

### Filtering Dates with the BETWEEN Operator

The `BETWEEN` operator filters for numeric or date values within a specified range.

- **Example: Identifying Machines Patched Between Dates**
    
    We'll construct a query to find all machines patched between March 1st, 2021, and September 1st, 2021.
    

2. **SQL Query Construction:**
    
    - Start by selecting all records from the `machines` table:
        
        ```sql
        SELECT *
        FROM machines
        ```
        
    - Include the `BETWEEN` operator within the `WHERE` clause.
    
4. **Specifying the Date Range:**
    
    - Following `WHERE`, indicate the column for filtering (`OS_patch_date` in this case).
    - Employ `BETWEEN` followed by the beginning of the range, the `AND` keyword, and then the end of the range.
        
        ```sql
        WHERE OS_patch_date BETWEEN '2021-03-01' AND '2021-09-01'
        ```
        
    
6. **Running the Query:**
    
    - Execute the query to observe the results, presenting a list of machines patched between the specified dates.
    

### Important Note: String vs. Numeric Data Filtering

Remember that quotation marks are used to enclose strings, dates, and times within filters. Numeric values, however, do not require quotation marks.

By mastering these techniques, you're well-equipped to construct diverse filters for numeric and date/time data within your SQL queries. The next session will cover advanced filtering using multiple conditions in a single query.

## Operators for filtering dates and numbers

This guide revisits operators used for filtering numeric and date/time data in SQL, emphasizing their significance for security analysts.

### Numbers, Dates, and Times in Cybersecurity

Security analysts delve into various data types beyond just strings. Numeric and date/time data play a crucial role in security investigations.

- **Examples of Numeric Data for Security Analysts:**
    
    - Number of login attempts
    - Count of specific log entries
    - Volume of data transferred (incoming/outgoing)
    
- **Examples of Date/Time Data for Security Analysts:**
    
    - Login timestamps within logs
    - Login dates
    - Patch application dates
    - Connection durations
    

### Comparison Operators for Filtering

- **Operators Commonly Used in Filters:**
    
    - `<` (Less Than)
    - `>` (Greater Than)
    - `=` (Equal To)
    - `<=` (Less Than or Equal To)
    - `>=` (Greater Than or Equal To)
    - `<>` (Not Equal To) (alternative: `!=`)
    
- **Using Operators in the WHERE Clause:**
    
    - These operators are incorporated within the `WHERE` clause at the query's end.
        
    - Example: Filtering for employees born after January 1st, 1970:
        
        ```sql
        SELECT firstname, lastname, birthdate
        FROM employees
        WHERE birthdate > '1970-01-01';
        ```
        
    - **Explanation:** This query retrieves first names, last names, and birthdates of employees born after (but not on) January 1st, 1970.
        
    
- **Inclusive vs. Exclusive Operators:**
    
    - `>` (Exclusive): Excludes the value being compared to.
    - `>=` (Inclusive): Includes the value being compared to.
    

### The BETWEEN Operator for Ranges

- **Filtering Within a Range:**
    
    - The `BETWEEN` operator filters numeric or date/time data falling within a specified range.
    
- **Example: Identifying Employees Hired Between Dates:**
    
    
```sql
      SELECT firstname, lastname, hiredate
      FROM employees
      WHERE hiredate BETWEEN '2002-01-01' AND '2003-01-01';
```
    
    
    - **Explanation:** This query filters for employees hired between January 1st, 2002, and January 1st, 2003 (inclusive).
    

### Key Takeaways

- Operators are instrumental for filtering numeric and date/time data in SQL.
- Grasp the distinction between exclusive (`<`, `>`) and inclusive (`<=`, `>=`) operators.
- The `BETWEEN` operator efficiently retrieves data within a specific range.

## Filters with AND, OR, and NOT

This guide equips you with the powerful trio of operators (AND, OR, and NOT) for crafting intricate filtering conditions within your SQL queries, empowering security analysts to target specific data combinations.

### The Need for Multi-Condition Filtering

Prior lessons explored filtering for single conditions. Real-world security scenarios often necessitate filtering based on multiple criteria. For instance, a security vulnerability might be contingent on factors like a specific operating system and email client combination. To identify potentially vulnerable machines, we must filter for machines using both the designated email client and operating system.

### The AND Operator: Ensuring All Conditions Are Met

- **Function:** The `AND` operator guarantees that both specified conditions must be satisfied simultaneously.
- **Analogy:** Imagine selecting apples from a large container. You want only "large AND fresh" apples. This eliminates small apples (even if fresh) and rotten apples (even if large). The result includes only large and fresh apples, meeting both conditions.

### Implementing AND in SQL

- **Example:** Filtering Machines Based on Operating System and Email Client

We aim to retrieve a list of machines running Operating System (OS) 1 and using Email Client 1.

```sql
SELECT *
FROM machines
WHERE operating_system = 'OS 1'
  AND email_client = 'Email Client 1';
```

- **Breakdown:**
    
    2. The `WHERE` clause specifies the filtering conditions.
    4. The first condition ensures the `operating_system` column has the value "OS 1."
    6. The `AND` operator connects this condition to another.
    8. The second condition requires the `email_client` column to have the value "Email Client 1."
    

### The OR Operator: Selecting Based on Any Condition

- **Function:** The `OR` operator signifies that either of the defined conditions can be met.
- **Analogy:** Imagine selecting entries where a circle represents a condition. Using `OR` in a Venn diagram instructs SQL to select all rows satisfying one or both conditions.

### Implementing OR in SQL

- **Example:** Identifying Machines Requiring a Patch

Let's filter for machines needing a patch, targeting those with either OS 1 or OS 3.


```sql
SELECT *
FROM machines
WHERE operating_system = 'OS 1'
  OR operating_system = 'OS 3';
```

- **Breakdown:**
    
    2. The `WHERE` clause houses the filtering conditions.
    4. The first condition targets machines with "OS 1."
    6. The `OR` operator connects this condition to another.
    8. The second condition targets machines with "OS 3."
    

### The NOT Operator: Excluding Specific Conditions

- **Function:** The `NOT` operator negates a condition.
- **Analogy:** Imagine selecting fruits that are not apples. This is more efficient than listing every desired fruit (banana, orange, etc.).

### Implementing NOT in SQL

- **Example:** Updating Devices Except Those Using OS 3

We intend to update all devices except those running OS 3.

```sql
SELECT *
FROM machines
WHERE NOT operating_system = 'OS 3';
```

- **Breakdown:**
    
    2. The `WHERE` clause introduces the filtering condition.
    4. The `NOT` operator precedes the condition to be negated.
    6. The condition excludes machines with "OS 3."
    

By mastering these operators (AND, OR, and NOT), you can construct sophisticated filtering conditions in your SQL queries, allowing you to extract precise data sets for security analysis.

## More on filters with AND, OR, and NOT

This session delves deeper into leveraging AND, OR, and NOT operators to craft meticulous filters within your SQL queries, empowering security analysts to pinpoint specific data relevant to investigations.

### Logical Operators: The Foundation for Granular Filtering

- **AND, OR, and NOT:** These operators, categorized as logical operators, enable security analysts to refine their SQL queries, retrieving only the information crucial for their work.

### The AND Operator: Ensuring Both Conditions Are Met

- **Function:** The `AND` operator guarantees that both specified conditions are satisfied simultaneously.
- **Example:** Identifying Customers Affected by a Security Concern

Imagine a security issue impacting only customer accounts handled by a support representative with ID 5 and located in the USA. To target these specific customers, we would use the `AND` operator within the `WHERE` clause:

```sql
SELECT firstname, lastname, email, country, supportrepid
FROM customers
WHERE supportrepid = 5 AND country = 'USA';
```

- **Explanation:** This query retrieves first names, last names, emails, countries, and support representative IDs, filtered to include only customers meeting both conditions (support rep ID 5 and USA location).

### The OR Operator: Selecting Based on Any Condition

- **Function:** The `OR` operator signifies that at least one of the defined conditions must be met.
- **Example:** Finding Customers for a Security Update

Let's say you need to notify all customers in either the USA or Canada about a security update. The `OR` operator facilitates retrieving the necessary records:

```sql
SELECT firstname, lastname, email, country
FROM customers
WHERE country = 'Canada' OR country = 'USA';
```

- **Explanation:** This query retrieves first names, last names, emails, and countries, encompassing all customers residing in either Canada or the USA.

### The NOT Operator: Excluding Specific Conditions

- **Function:** The `NOT` operator negates a condition, returning entries that do not fulfill that condition.
- **Example:** Identifying Customers Not Affected by a Security Issue

Suppose a security concern doesn't affect customers in the USA, but might impact those in other countries. We can efficiently target non-US customers using the `NOT` operator:

```sql
SELECT firstname, lastname, email, country
FROM customers
WHERE NOT country = 'USA';
```

- **Explanation:** This query retrieves first names, last names, emails, and countries, encompassing all customers excluding those located in the USA.

**Pro Tip:** Alternative operators (`<>` or `!=`) can also be used to specify values that are not equal to a certain value.

### Combining Logical Operators for Complex Queries

Logical operators can be combined to construct intricate filters. For instance, if neither the USA nor Canada is affected by a security issue, we can combine operators to target customers in all other countries:

```sql
SELECT firstname, lastname, email, country
FROM customers
WHERE NOT country = 'Canada' AND NOT country = 'USA';
```

- **Explanation:** The `NOT` operator precedes the first condition (Canada). It's then joined to the second condition (USA) using `AND`, ensuring both exclusions are met. This query retrieves customer information for all countries except Canada and the USA.

### Key Takeaways

Logical operators are instrumental in creating specific filters tailored to extract security-related data. Remember:

- `AND`: Both conditions must be true.
- `OR`: Either one or both conditions can be true.
- `NOT`: The specified condition is negated (excluded).
- Logical operators can be combined for even more targeted queries.

By mastering these operators, you'll be well-equipped to construct refined SQL queries, enabling you to gather the precise data required for thorough security analyses.

# SQL joins

## Join tables in SQL

This guide unveils the concept of joining tables in SQL, empowering you to seamlessly combine data from various tables within a database. This capability is particularly valuable for security analysts when information resides in separate tables.

### Introduction to Joins

Imagine possessing two tables:

- One detailing security vulnerabilities within various operating systems.
- Another containing information about your company's machines, including their operating systems.

By joining these tables, you can generate a comprehensive list of vulnerable machines within your network – a powerful tool for security professionals.

### Table Joins: Unifying Data Through Shared Columns

- **Challenge:** When working with two tables, SQL requires clarity regarding the table from which you're selecting columns.
- **Solution:** Specify the table name, followed by a period (.), and then the column name (e.g., `employees.employee_id`). This approach precisely identifies the intended column.

### Joining Tables: A Practical Example

- **Scenario:** Gaining insights into which employees are accessing specific machines within your organization.
    
- **Solution:** Joining the `employees` and `machines` tables using a shared column (often a primary key in one table and a foreign key in the other).
    
- **Primary Key:** A unique identifier within a table, ensuring no duplicate values exist.
    
- **Foreign Key:** A column referencing a primary key in another table, establishing a relationship between them.
    
- **Example:** Let's assume `employee_id` acts as the primary key in the `employees` table and a foreign key in the `machines` table.
    

### Unveiling the INNER JOIN

- **Function:** An INNER JOIN retrieves rows that possess matching values in a specified column present in both tables.
    
- **Understanding INNER JOIN:**
    
    - Consider a reduced dataset with four rows from each table (`employees` and `machines`), focusing on a few relevant columns.
    - If `employee_id` is chosen for the join, rows containing matching `employee_id` values (e.g., 1188 and 1189) in both tables are considered matches.
    - The outcome of the join incorporates these matching rows, encompassing all columns from both tables.
    
- **Handling NULL Values:** NULL signifies missing data entries within SQL. It might represent unassigned machines (no designated employee).
    

### Implementing Joins in SQL

- **Example:** Joining `employees` and `machines` tables to retrieve a list containing usernames, office locations, and operating systems used on assigned machines.

SQL

```
SELECT username, office, operating_system
FROM employees
INNER JOIN machines ON employees.employee_id = machines.employee_id;
```

- **Breakdown:**
    
    - `SELECT`: Specifies the desired columns from the tables.
    - `FROM employees`: Indicates the starting table (left table) for the join.
    - `INNER JOIN`: Instructs SQL to perform an inner join.
    - `machines`: Names the second table (right table) to be joined.
    - `ON`: Introduces the condition for joining the tables.
    - `employees.employee_id = machines.employee_id`: Specifies the columns used for the join (matching employee IDs in both tables).
    
- **Result:** This query successfully joins the two tables, delivering records with matching employee IDs. The output showcases data from both tables, limited to the columns chosen in the `SELECT` clause.
    

### Conclusion

By mastering joins, you can effortlessly combine data from multiple tables within your SQL queries, empowering you to extract valuable insights for security analysis. The next lesson will delve into other join types that extend your capabilities for working with related tables.

## Types of joins

In SQL, outer joins expand on the concept of inner joins by including all entries from one or both tables, regardless of matches in specified columns. Let's explore the three types of outer joins: LEFT JOIN, RIGHT JOIN, and FULL OUTER JOIN.

### Introduction to Outer Joins

Outer joins are beneficial when complete data from one or both tables is needed, even without exact matches in joining columns.

#### Types of Outer Joins

1. **LEFT JOIN:**
   - Returns all records from the first table.
   - Includes matching rows from the second table.
   - Non-matching rows from the first table contain NULL values for columns from the second table.

2. **RIGHT JOIN:**
   - Returns all records from the second table.
   - Includes matching rows from the first table.
   - Non-matching rows from the second table contain NULL values for columns from the first table.

3. **FULL OUTER JOIN:**
   - Returns all records from both tables.
   - Includes NULL values for unmatched columns in either table.

### Exploring Outer Joins

Let's dive into each type of outer join with illustrative examples.

#### LEFT JOIN

Consider tables `employees` (left) and `machines` (right), joined on `employee_id`. 

```sql
SELECT *
FROM employees
LEFT JOIN machines ON employees.employee_id = machines.employee_id;
```

- Returns all records from `employees`.
- Includes matching rows from `machines`.
- Non-matching rows from `employees` contain NULL values for `machines` columns.

#### RIGHT JOIN

Using the same tables but with a RIGHT JOIN:

```sql
SELECT *
FROM employees
RIGHT JOIN machines ON employees.employee_id = machines.employee_id;
```

- Returns all records from `machines`.
- Includes matching rows from `employees`.
- Non-matching rows from `machines` contain NULL values for `employees` columns.

#### FULL OUTER JOIN

For a FULL OUTER JOIN on the same tables:

```sql
SELECT *
FROM employees
FULL OUTER JOIN machines ON employees.employee_id = machines.employee_id;
```

- Returns all records from both tables.
- Includes NULL values for unmatched columns in either table.

### Syntax for Outer Joins

Implementing outer joins in SQL uses a similar structure as inner joins but with specific keywords:

- `LEFT JOIN`
- `RIGHT JOIN`
- `FULL OUTER JOIN`

```sql
SELECT columns
FROM table1
LEFT/RIGHT/FULL OUTER JOIN table2 ON table1.column = table2.column;
```

### Conclusion

Understanding outer joins is vital for comprehensive data retrieval in SQL. Each type offers distinct advantages based on the required data set.

## Compare types of joins

SQL offers various join types to merge data from multiple tables. Let's compare and analyse the syntax for each type of join.

### Inner Joins

Inner joins focus on returning rows that have matching values in specified columns from both tables.

#### Inner Join Syntax

```sql
SELECT *
FROM employees
INNER JOIN machines ON employees.device_id = machines.device_id;
```

- Specify the two tables to join (`employees` and `machines`).
- Use `INNER JOIN` keyword.
- Connect tables on a common column (`device_id`).

### Outer Joins

Outer joins expand join results to include all rows from one or both tables, even if no match exists.

#### Left Join

Left joins return all records from the left table and matching rows from the right table.

```sql
SELECT *
FROM employees
LEFT JOIN machines ON employees.device_id = machines.device_id;
```

- All records from `employees`.
- Only matching rows from `machines`.
- Non-matching rows from `machines` have NULL values.

#### Right Join

Right joins are similar to left joins but prioritize all records from the right table.

```sql
SELECT *
FROM employees
RIGHT JOIN machines ON employees.device_id = machines.device_id;
```

- All records from `machines`.
- Only matching rows from `employees`.
- Non-matching rows from `employees` have NULL values.

#### Full Outer Join

Full outer joins return all records from both tables, merging them completely.

```sql
SELECT *
FROM employees
FULL OUTER JOIN machines ON employees.device_id = machines.device_id;
```

- All records from both `employees` and `machines`.
- NULL values for unmatched columns in either table.

### Key Differences

- **INNER JOIN:** Returns only matching records.
- **LEFT JOIN:** Returns all from left table + matching from right.
- **RIGHT JOIN:** Returns all from right table + matching from left.
- **FULL OUTER JOIN:** Returns all from both tables.

### Table Summary

| Join Type       | Description                                      | Example Syntax                                              |
|-----------------|--------------------------------------------------|--------------------------------------------------------------|
| Inner Join      | Returns matching records from both tables        | `INNER JOIN employees ON employees.device_id = machines.device_id;` |
| Left Join       | Returns all from left + matching from right      | `LEFT JOIN employees ON employees.device_id = machines.device_id;`  |
| Right Join      | Returns all from right + matching from left      | `RIGHT JOIN employees ON employees.device_id = machines.device_id;` |
| Full Outer Join | Returns all from both tables                     | `FULL OUTER JOIN employees ON employees.device_id = machines.device_id;` |

Understanding these join types and their syntax empowers you to manipulate data effectively in SQL.

## Continuous learning in SQL

### Overview
Aggregate functions in SQL are powerful tools that perform calculations over multiple data points and return summarized results rather than individual records. This section delves into the syntax and usage of aggregate functions like COUNT, AVG, and SUM.

### Aggregate Function Types
Here are some common aggregate functions and their purposes:

| Function | Purpose                                              |
|----------|------------------------------------------------------|
| COUNT    | Returns the number of rows in a result set           |
| AVG      | Calculates the average of numerical data in a column  |
| SUM      | Computes the sum of numerical data in a column        |

### Aggregate Function Syntax
To use an aggregate function in SQL, follow this syntax:

```sql
SELECT aggregate_function(column_name) 
FROM table_name 
WHERE conditions;
```

For example, to count the number of customers in the `customers` table, you would use:

```sql
SELECT COUNT(firstname)
FROM customers;
```

### Filtering Aggregate Functions
You can combine aggregate functions with filters to get specific results. For instance, to count the number of customers from the USA:

```sql
SELECT COUNT(firstname)
FROM customers
WHERE country = 'USA';
```

### Continuing Your SQL Learning Journey
After mastering aggregate functions, you can further your SQL knowledge in several ways:

1. **Self-Study:** Explore online resources and tutorials dedicated to SQL.
2. **Practical Experience:** Apply SQL in real-world scenarios to reinforce your skills.
3. **Problem-Solving:** Tackle complex queries and challenges to deepen your understanding.
4. **Online Communities:** Engage with SQL communities for support and knowledge sharing.

### Key Takeaways
- Aggregate functions enable data summarization in SQL.
- Combine aggregate functions with filters for precise results.
- Continual learning and practical application enhance SQL proficiency.
- Online resources and communities provide ongoing support for SQL learners.

---
## Glossary terms from module 4


**Database**: An organized collection of information or data

**Date and time data:** Data representing a date and/or time

**Exclusive operator**: An operator that does not include the value of comparison

**Filtering:** Selecting data that match a certain condition

**Foreign key:** A column in a table that is a primary key in another table 

**Inclusive operator:** An operator that includes the value of comparison

**Log:** A record of events that occur within an organization's systems

**Numeric data:** Data consisting of numbers

**Operator:** A symbol or keyword that represents an operation

**Primary key:** A column where every row has a unique entry

**Query:** A request for data from a database table or a combination of tables

**Relational database:** A structured database containing tables that are related to each other

**String data**: Data consisting of an ordered sequence of characters

**SQL (Structured Query Language):** A programming language used to create, interact with, and request information from a database

**Syntax:** The rules that determine what is correctly structured in a computing language

**Wildcard**: A special character that can be substituted with any other character