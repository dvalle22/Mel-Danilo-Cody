---
layout: default
title: Create a schema
parent: Schema and Table Setup
nav_order: 1
---

# Create a schema

1. Open your Workbench. If you have set it up correctly, a MySQL Local instance will appear on the homepage.
    
    ![MySQL Workbench homepage with local instance](https://github.com/dvalle22/Mel-Danilo-Cody/blob/gh-pages/assets/images/local-instance-hightlighted.png?raw=true)
    
2. Double click on Local instance. A login popup window will appear. Enter your username and password, then press OK to proceed.
    
    ![MySQL Workbench login](https://github.com/dvalle22/Mel-Danilo-Cody/blob/gh-pages/assets/images/login.png?raw=true)
    {: style="width: 300px;" }
    
        ⚠️: You cannot use MySQL Workbench if you skip this step.
        > Connecting to a local instance will grant you access to your MySQL database.
    
    Once successfully logged in, you will see this layout.
    
    ![MySQL Workbench login successfully](https://github.com/dvalle22/Mel-Danilo-Cody/blob/gh-pages/assets/images/workbench-layout-no-annotation.png?raw=true)

3. In the top left corner of Workbench, click on the icon with the word 'SQL' and a '+' sign.

    ![MySQL Workbench add new query button](https://github.com/dvalle22/Mel-Danilo-Cody/blob/gh-pages/assets/images/open-new-query-tab.png?raw=true)
    {: style="width: 500px;" }
    
    A SQL tab will appear in the middle of the MySQL Workbench layout. This is the place where you add and execute all of your SQL queries.
    
    ![MySQL Workbench new query](https://github.com/dvalle22/Mel-Danilo-Cody/blob/gh-pages/assets/images/new-query-tab.png?raw=true)
    
4. Copy and paste this line of SQL code into the newly created SQL file.
    
     ```sql
    CREATE SCHEMA IF NOT EXISTS user_demo;
    ```
    
5. Click the thunder icon at the top of the SQL tab to execute the SQL file.
    
    ![MySQL Workbench run query button](https://github.com/dvalle22/Mel-Danilo-Cody/blob/gh-pages/assets/images/execute-query-button.png?raw=true)
    
        ⚠️: This icon will execute every SQL query that exists in the SQL file.
        > Make sure you write the queries correctly before clicking this icon.
    
    After executing the SQL queries, the Output tab below will show the status of the execution. If you see the green checkmark, the queries have run successfully.
    
    ![MySQL Workbench run query result](https://github.com/dvalle22/Mel-Danilo-Cody/blob/gh-pages/assets/images/execute-query-result.png?raw=true)

    Your schema has been created. However, it has not shown up in the Schemas tab. Therefore, you need to reload the Schemas tab.
    
6. Hover your cursor over the Schemas tab. Right click and select 'Refresh All'.
    
    ![MySQL Workbench update schema](https://github.com/dvalle22/Mel-Danilo-Cody/blob/gh-pages/assets/images/update-schema.png?raw=true)

    The newly created schema will now appear in the Schemas tab.

    ![MySQL Workbench show new schema](https://github.com/dvalle22/Mel-Danilo-Cody/blob/gh-pages/assets/images/update-schema-show-up.png?raw=true)
    
    Next, we will create our first table inside this new schema, 'user_demo'.
