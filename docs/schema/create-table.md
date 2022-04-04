---
layout: default
title: Create a table
parent: Schema Setup and Adding Tables
nav_order: 2
---

# Create a table

Now that you have already had a schema 'user_demo', the next step is creating a table inside that schema to start storing your data.

In this tutorial, you will be a teacher who needs to keep a record of students who are the users of a forum you that own. Each student will have to enter a numeric ID, first name, last name, date of birth, gender, email, and the program they are currently enrolled.

With this information, let's create your 'User' table.

1. A table needs a schema to locate on. After creating a schema, you need to manually selected that schema to be the current schema. Check if you are inside a schema by looking at the Schemas tab.
    ![MySQL Workbench no schema selected](https://github.com/dvalle22/Mel-Danilo-Cody/blob/gh-pages/assets/images/no-schema-selected.png?raw=true)
    
    If no name is in bold, it means that you are not currently inside any schema.
    
2. In the Schemas tab, hover over 'user_demo' and double click on the name. After this, 'user_demo' will turn bold, indicating that it is selected as the current schema.
    
    ![MySQL Workbench schema selected](https://github.com/dvalle22/Mel-Danilo-Cody/blob/gh-pages/assets/images/schema-selected.png?raw=true)
    
3. Copy and paste this line of SQL code into the SQL file opened in your Workbench.
    
    ```sql
    CREATE TABLE `User` (
        `id` int NOT NULL,
        `fName` varchar(80) NOT NULL,
        `lName` varchar(80) NOT NULL,
        `DoB` date NOT NULL,
        `gender` ENUM('Male', 'Female'),
        `email` varchar(100),
        `program` ENUM('Computing', 'Accounting', 'Business', 'Engineering') NOT NULL,
        PRIMARY KEY (`id`)
    )
    ```

        📖: SQL supports these data types:
            - int: an integer number
            - double: a floating point number
            - varchar(size): a string
            - date: a date in YYYY-MM-DD format
            - enum: a string that is chosen from a list of possible values.
      
    For more data types, visit [MySQL Workbench tips](docs/tips)
    
4. Click the thunder icon at the top of the SQL tab to execute the SQL file.
    
        ⚠️: If you keep the line `CREATE SCHEMA IF NOT EXISTS user_demo;`, your Output tab will print a warning message.
        > This is because MySQL detects that there is potentially two schemas with the same name. This is not an error, because the keyword 'IF NOT EXISTS' prevents this from happening.
        > However, deleting the keyword 'IF NOT EXISTS' will result in an error and a red 'X' mark will appear in the Output tab. 
    
    Your table has been created. However, it has not showed up in the Schemas tab. Therefore, we need to reset the Schemas tab.
    
5. Hovering your cursor over the Schemas tab. Right click and select 'Refresh All'.
    
    ![MySQL Workbench update table](https://github.com/dvalle22/Mel-Danilo-Cody/blob/gh-pages/assets/images/update-table.png?raw=true)
    
    After this, you will see a triangle appear to the left of 'Tables' under 'user_demo'. Click on the triangle to see the table 'User' underneath.
    
    ![MySQL Workbench table updated](https://github.com/dvalle22/Mel-Danilo-Cody/blob/gh-pages/assets/images/update-table-show-up.png?raw=true)
    
6. Check if you have created the correct table by double clicked on 'User' under 'Tables' under 'user_demo'. The Information tab below will display the columns in 'User'. Make sure it match with the data types we specify in the code before proceeding to the next section [Query to Display Data](docs/display).
    
    ![MySQL Workbench see new table](https://github.com/dvalle22/Mel-Danilo-Cody/blob/gh-pages/assets/images/update-table-show-details.png?raw=true)
    
