---
layout: default
title: Query to Modify Data
nav_order: 4
---

# Query to Modify Data
After creating a table in MySQL, you are able to add data to the table by writing a query, by using the [INSERT INTO](https://dvalle22.github.io/Mel-Danilo-Cody/) statement.

Copy the code sample below, and try running it on your own MySQL workbench:

```sql
INSERT INTO `User` (`id`, `fName`, `lName`, `DoB`, `gender`, `email`, `program`) VALUES
(9734109, 'Eduard', 'Khil', '2001-12-22', 'Male', 'trolleyguy@gmail.com', 'Computing'),
(9734512, 'Mikhail', 'Mishustin', '2003-09-16', 'Male', 'mikki.mishutin@hotmail.com', 'Accounting'),
(19084223, 'Lucy', 'Ali', '1994-02-01', 'Female', 'lucy.ali1@uq.edu.au', 'Business'),
(19087623, 'John', 'Monarch', '1995-01-06', 'Male', 'john.monarch@uq.edu.au', 'Computing'),
(19088623, 'Ursula', 'Smith', '1997-07-09', 'Female', 'u.smith@qut.edu.au', 'Computing'),
(19088644, 'Marcus', 'Jacobs', '1999-06-04', 'Male', NULL, 'Accounting'),
(19439623, 'Nevena', 'Ivanovic', '2000-12-21', 'Female', 'Nevena@gmail.com', 'Business'),
(19488623, 'Leo', 'Montgomery', '1989-01-01', 'Male', 'leolovescars@gmail.com', 'Engineering'),
(19609863, 'Edi', 'Rama', '1987-03-03', 'Male', 'edi.rama@uq.edu.au', 'Computing'),
(22732951, 'Jamie', 'Sleeman', '1999-06-29', 'Male', NULL, 'Engineering'),
(23982121, 'Hye-sun', 'Ku', '1998-07-04', 'Female', 'ku@uq.edu.au', 'Engineering'),
(23987721, 'Min-ho', 'Lee', '2001-05-23', 'Female', 'lee@uq.edu.au', 'Business'),
(38982921, 'Jeong-hyeok', 'Ri', '2002-06-22', NULL, 'ri.jonghyok@hotmail.com', 'Accounting'),
(41284471, 'Bong-soon', 'Park', '1994-08-06', 'Male', 'park.bongsoon@ainsoft.com', 'Computing'),
(42180081, 'Se-ri', 'Yoon', '1994-04-5', 'Female', 'yoon.seri@queen.com', 'Engineering'),
(66234500, 'Sven', 'Kirsch', '1999-05-13', 'Male', 'sven.kirsch@uq.edu.au', 'Engineering'),
(66234591, 'Matthieu', 'Loiselle', '2002-08-14', NULL, 'matt.loiselle@uq.edu.au', 'Accounting'),
(66234592, 'Gabriel', 'Duperre', '2001-07-24', 'Male', 'Gabe.dupe@gmail.comm', 'Accounting'),
(66234593, 'Honore', 'Avare', '1991-06-25', 'Male', 'honore@hotmail', 'Accounting'),
(66234594, 'Margit', 'Gade', '1993-04-24', 'Female', 'margit.gade1@uq.edu.au', 'Business'),
(66234595, 'Lavinia', 'Pinto', '1992-01-19', 'Male', 'lavinia@hotmail.com', 'Business');
```

To see if you've succesfully added the provided data into your table, you can write a simple query:

```sql
SELECT * FROM user_demo.user;
```

Alternatively, right-click the user table, and click on the first option **SELECT ROWS - LIMIT 1000**.
After running the query, you should see a Result Grid made up of every column in the user table.

![MySQL full_user_table](https://github.com/dvalle22/Mel-Danilo-Cody/blob/gh-pages/assets/images/table_screenshot.png?raw=true)
{: style="height: 800px;
  width: 800px;" }
## Header 2
