[![HTML](https://img.shields.io/badge/-HTML-orange?style=flat-square)](https://github.com/nayemspecial/wordpress-support-engineer/blob/main/assets/01.HTML/html-course-outline.md)
[![CSS](https://img.shields.io/badge/-CSS-blue?style=flat-square)](https://github.com/nayemspecial/wordpress-support-engineer/blob/main/assets/02.CSS/css-course-outline.md)
[![JavaScript](https://img.shields.io/badge/-JavaScript-yellow?style=flat-square)](https://github.com/nayemspecial/wordpress-support-engineer/blob/main/assets/03.JavaScript/course-module.md)
[![Tailwind CSS](https://img.shields.io/badge/-Tailwind_CSS-38B2AC?style=flat-square&logo=tailwind-css&logoColor=white)](https://github.com/nayemspecial/wordpress-support-engineer/blob/main/assets/04.TailwindCSS/course-module.md)
[![PHP](https://img.shields.io/badge/-PHP-777BB4?style=flat-square&logo=php&logoColor=white)](https://github.com/nayemspecial/wordpress-support-engineer/blob/main/assets/07.PHP/module2.md)
[![MySQL](https://img.shields.io/badge/-MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white)](https://github.com/nayemspecial/wordpress-support-engineer/blob/main/assets/08.MySQL/mysql-course-module.md)
[![WordPress](https://img.shields.io/badge/-WordPress-21759B?style=flat-square&logo=wordpress&logoColor=white)]()

- [ ] **ক্লাস ০১ কন্টেন্ট এখান থেকে শুরু এবং** [ক্লাস ভিডিও এখানে](https://youtu.be/ykp8A_xiIdg)
### ১। SQL ও RDBMS এর পরিচিতি
- [ ] ডেটাবেজ কী?
- [ ] টেবিল কী?
- [ ] টেবিল রো 
- [ ] টেবিল কলাম
- [ ] ডেটাবেজ টেবিল
- [ ] রেকর্ড, ফিল্ড
- [ ] রিলেশনাল ডেটাবেজ কী?
- [ ] RDBMS এর বৈশিষ্ট্য ও উপকারিতা
- [ ] প্রাইমারি কী
- [ ] ফরেন কী
- [ ] কম্পোজিট প্রাইমারি কী
- [ ] প্রয়োজনীয় টুলস
    - [ ] লারাগন লোকাল সার্ভার
    - [ ] phpmyadmin

### ২। SQL সিনট্যাক্স ও গঠন
- [ ] SQL স্টেটমেন্ট লেখার নিয়ম
- [ ] SQL কেস ইনসেনসিটিভ
- [ ] সেমিকোলনের ব্যবহার

### ৩। ডেটা ডেফিনিশন ল্যাংগুয়েজ (DDL)
- [ ] CREATE DATABASE
- [ ] CREATE TABLE
- [ ] INSER INTO
- [ ] ALTER TABLE – ADD COLUMN
- [ ] ALTER TABLE – MODIFY COLUMN
- [ ] ALTER TABLE – DROP COLUMN

- [ ] **ক্লাস ০২ কন্টেন্ট এখান থেকে শুরু এবং** [ক্লাস ভিডিও এখানে]()

- [ ] SELECT দিয়ে সমস্ত ডেটা দেখানো  
      `SELECT * FROM customers;`

- [ ] নির্দিষ্ট কলাম (firstName, lastName) দেখানো  
      `SELECT firstName, lastName FROM customers;`

- [ ] CONCAT দিয়ে ফুলনেম তৈরি করা (AS সহ)  
      `SELECT CONCAT(firstName, ' ', lastName) AS fullName FROM customers;`

- [ ] WHERE দিয়ে একটি শহরের ডেটা ফিল্টার করা (e.g., Dhaka)  
      `SELECT * FROM customers WHERE city = 'Dhaka';`

- [ ] একাধিক শর্ত দিয়ে ডেটা ফিল্টার করা (AND কন্ডিশন)  
      `SELECT * FROM customers WHERE city = 'Dhaka' AND lastName = 'Rahman';`

- [ ] BETWEEN দিয়ে ID রেঞ্জে ফিল্টার করা  
      `SELECT * FROM customers WHERE id BETWEEN 10 AND 20;`

- [ ] IN দিয়ে একাধিক শহর সিলেক্ট করা  
      `SELECT * FROM customers WHERE city IN ('Dhaka', 'Khulna', 'Sylhet');`

- [ ] LIKE দিয়ে পারশিয়াল ইমেইল খোঁজা  
      `SELECT * FROM customers WHERE email LIKE '%rahman%';`

- [ ] ORDER BY দিয়ে নাম অনুযায়ী সাজানো (ASC/Descending)  
      `SELECT * FROM customers ORDER BY firstName ASC;`

- [ ] LIMIT দিয়ে সর্বশেষ ১০টি রেকর্ড দেখানো  
      `SELECT * FROM customers ORDER BY id DESC LIMIT 10;`

- [ ] DISTINCT দিয়ে ইউনিক সিটি লিস্ট দেখানো  
      `SELECT DISTINCT city FROM customers;`

- [ ] LIKE দিয়ে S দিয়ে শুরু হওয়া নাম খোঁজা  
      `SELECT * FROM customers WHERE firstName LIKE 'S%';`

- [ ] IS NOT NULL দিয়ে address যেটা null নয় এমন ডেটা ফিল্টার করা  
      `SELECT * FROM customers WHERE address IS NOT NULL;`

- [ ] Calculated কলাম তৈরি করা (id * 10)  
      `SELECT id, firstName, id * 10 AS custom_id FROM customers;`

- [ ] LIMIT দিয়ে শুধুমাত্র ৫টি নাম ও শহর দেখানো  
      `SELECT firstName, city FROM customers LIMIT 5;`

- [ ] নাম অনুসারে সাজিয়ে প্রথম ১০টি রেকর্ড দেখানো  
      `SELECT * FROM customers ORDER BY firstName LIMIT 10;`

- [ ] Dhaka শহরের কাস্টমারদের ইমেইল দেখানো  
      `SELECT email FROM customers WHERE city = 'Dhaka';`

- [ ] '001' দিয়ে শেষ হয় এমন ফোন নাম্বার খোঁজা  
      `SELECT * FROM customers WHERE phone LIKE '%001';`

- [ ] UPPER ও LOWER ফাংশন ব্যবহার করে কেস পরিবর্তন  
      `SELECT UPPER(firstName), LOWER(email) FROM customers;`

- [ ] নামের দৈর্ঘ্য (LENGTH) বের করা  
      `SELECT firstName, LENGTH(firstName) AS name_length FROM customers;`

- [ ] UPDATE
- [ ] UPDATE WHERE
- [ ] DELETE FROM
- [ ] DELETE WITH JOIN
- [ ] REPLACE INTO
- [ ] MERGE (Applicable case)

### ৫। Aggregate Functions ও Grouping
- [ ] SUM
- [ ] AVG
- [ ] MIN
- [ ] MAX
- [ ] COUNT
- [ ] GROUP BY
- [ ] HAVING
- [ ] COUNT DISTINCT

### ৬। Constraints ও Keys
- [ ] PRIMARY KEY
- [ ] COMPOSITE PRIMARY KEY
- [ ] FOREIGN KEY
- [ ] ON DELETE/UPDATE CASCADE
- [ ] UNIQUE
- [ ] NOT NULL
- [ ] DEFAULT
- [ ] CHECK
- [ ] ENUM constraint
- [ ] AUTO_INCREMENT
- [ ] CONSTRAINT নামকরণ
- [ ] DROP CONSTRAINT
- [ ] MODIFY CONSTRAINT

### ৭। JOIN অপারেশন
- [ ] INNER JOIN
- [ ] LEFT JOIN
- [ ] RIGHT JOIN
- [ ] FULL OUTER JOIN
- [ ] SELF JOIN
- [ ] CROSS JOIN
- [ ] NATURAL JOIN
- [ ] JOIN Performance Tips

### ৮। Subqueries
- [ ] Scalar Subquery
- [ ] Table Subquery
- [ ] Nested Subquery
- [ ] Correlated Subquery
- [ ] Subquery in WHERE
- [ ] Subquery in FROM
- [ ] Subquery in SELECT

### ৯। ফাংশন ও এক্সপ্রেশন
- [ ] CONCAT
- [ ] SUBSTRING
- [ ] UPPER / LOWER
- [ ] REPLACE
- [ ] LENGTH / CHAR_LENGTH
- [ ] NOW(), CURDATE(), CURTIME()
- [ ] DATEDIFF()
- [ ] DATE_ADD(), DATE_SUB()
- [ ] ROUND, FLOOR, CEIL, MOD
- [ ] CASE
- [ ] NULLIF
- [ ] COALESCE
- [ ] IF() function
- [ ] CAST(), CONVERT()

### ১০। Views
- [ ] CREATE VIEW
- [ ] ALTER VIEW
- [ ] DROP VIEW
- [ ] Updatable View
- [ ] Nested View
- [ ] View vs Table

### ১১। Indexes ও Query Optimization
- [ ] CREATE INDEX
- [ ] DROP INDEX
- [ ] UNIQUE INDEX
- [ ] EXPLAIN দিয়ে কুয়েরি বিশ্লেষণ
- [ ] Slow Query Log
- [ ] Execution Plan
- [ ] Covering Index
- [ ] Clustered vs Non-clustered Index
- [ ] Indexing Best Practices

### ১২। Transactions ও ACID
- [ ] START TRANSACTION
- [ ] COMMIT
- [ ] ROLLBACK
- [ ] SAVEPOINT
- [ ] RELEASE SAVEPOINT
- [ ] READ UNCOMMITTED
- [ ] READ COMMITTED
- [ ] REPEATABLE READ
- [ ] SERIALIZABLE
- [ ] Atomicity
- [ ] Consistency
- [ ] Isolation
- [ ] Durability

### ১৩। Security ও User Management
- [ ] CREATE USER
- [ ] GRANT PRIVILEGES
- [ ] REVOKE PRIVILEGES
- [ ] SHOW GRANTS
- [ ] WITH GRANT OPTION
- [ ] DROP USER
- [ ] SQL Injection প্রতিরোধ

### ১৪। Stored Procedures ও Functions
- [ ] CREATE PROCEDURE
- [ ] CALL PROCEDURE
- [ ] CREATE FUNCTION
- [ ] IN, OUT, INOUT Parameters
- [ ] DELIMITER ব্যবহার
- [ ] RETURN value
- [ ] SET Variable
- [ ] IF, CASE, WHILE, LOOP

### ১৫। Performance Optimization
- [ ] WHERE clause efficiency
- [ ] SELECT only required columns
- [ ] Avoid SELECT *
- [ ] Use LIMIT properly
- [ ] Indexing effectively
- [ ] Avoid unnecessary subqueries
- [ ] Partitioning

### ১৬। Advanced SQL
- [ ] Common Table Expressions (CTE)
- [ ] Recursive Query
- [ ] PIVOT / UNPIVOT
- [ ] ROW_NUMBER()
- [ ] RANK()
- [ ] DENSE_RANK()
- [ ] LEAD()
- [ ] LAG()
- [ ] Dynamic SQL
- [ ] JSON in MySQL
- [ ] Full Text Search
- [ ] Temporary Tables
