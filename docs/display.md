---
layout: default
title: Query to Display Data
nav_order: 5
---

# Query to Display Data
For this section we will be displaying a table from the database in MySQL Workbench. 

This tutorial works with the table used in [Query to Modify Data](https://dvalle22.github.io/Mel-Danilo-Cody/docs/modify/#query-to-modify-data) and also works with any tables on MySQL in general.

A visual representation of a table in MySQL will look like the following figure.

  ![MySQL Workbench visual table](https://github.com/dvalle22/Mel-Danilo-Cody/blob/gh-pages/assets/images/querydisplay/table_intro.png?raw=true)

As shown in the figure above, the column names are listed at the top followed by every row of student information inserted into the table.

Follow the steps below to acheive this.

1. In MySQL Workbench, click the 'Create a new SQL tab for executing queries' icon at the top left corner of the window as shown below. 
    
    ![MySQL Workbench new SQL query tab](https://github.com/dvalle22/Mel-Danilo-Cody/blob/gh-pages/assets/images/querydisplay/createsql_tab.png?raw=true)

    A blank text file should appear in the centre panel of MySQL Workbench.
    
    ![MySQL Workbench blank text file](https://github.com/dvalle22/Mel-Danilo-Cody/blob/gh-pages/assets/images/querydisplay/blank_textfile.png?raw=true)


2. Copy the block of code below
      ```sql
    SELECT *
    FROM user;
    ```


3. Paste the copied code into the blank text file. 
    
    ![MySQL Workbench code pasted to query file](https://github.com/dvalle22/Mel-Danilo-Cody/blob/gh-pages/assets/images/querydisplay/select_all_pasted.png?raw=true)
    
    The * here can be thought of the word 'all'.
    
    If you are using a different table you can replace _user_ from the copied code from Step 2.
    
    ![MySQL Workbench code pasted to query file different table name](https://github.com/dvalle22/Mel-Danilo-Cody/blob/gh-pages/assets/images/querydisplay/own_table.png?raw=true)
    

4. Click on the execute icon

    ![MySQL Workbench execute tab](https://github.com/dvalle22/Mel-Danilo-Cody/blob/gh-pages/assets/images/querydisplay/execute.png?raw=true)
    

5. View the table in the centre panel. 

    ![MySQL Workbench table is now visible](https://github.com/dvalle22/Mel-Danilo-Cody/blob/gh-pages/assets/images/querydisplay/table_appears.png?raw=true)
    
    Depending on your window size, you may need to hover your mouse over any of the four sides of the panel to readjust its size.
    
-------------------------------
Displaying the entire table can also be done through the MySQL Workbench graphical user interface.

1. Locate the 'Navigator' panel to the left for a list of your current schemas.

    ![MySQL Workbench navigator panel](https://github.com/dvalle22/Mel-Danilo-Cody/blob/gh-pages/assets/images/querydisplay/nav_panel.png?raw=true)

    If the 'Navigator' panel is not showing your current schemas, click on the 'Schemas' tab at the bottom of the panel to display a list of your schemas.
    
    ![MySQL Workbench administration and schemas tabs](https://github.com/dvalle22/Mel-Danilo-Cody/blob/gh-pages/assets/images/querydisplay/admin_and_schemas.png?raw=true)
    
2. Click on the arrow next to the schema containing the table you would like to display.

     Another list of items should appear directly underneath your schema, and the arrow next to the schema should be pointing down.

     ![MySQL Workbench sublist appears under schema](https://github.com/dvalle22/Mel-Danilo-Cody/blob/gh-pages/assets/images/querydisplay/schema_sublist.png?raw=true)

3. Click on the arrow next to the 'Tables' item to display the list of tables as we did in Step 2.
     
     ![MySQL Workbench tables list](https://github.com/dvalle22/Mel-Danilo-Cody/blob/gh-pages/assets/images/querydisplay/tables_list.png?raw=true)

4. Right click on the name of the table you would like to display.
    
    ![MySQL Workbench right clicking a table](https://github.com/dvalle22/Mel-Danilo-Cody/blob/gh-pages/assets/images/querydisplay/rightclick_table.png?raw=true)
    
    Click on 'Select Rows - Limit 1000'. A new tab with SQL code and a visual representation of the table will appear in the centre panel.
    
    ![MySQL Workbench visual table shown](https://github.com/dvalle22/Mel-Danilo-Cody/blob/gh-pages/assets/images/querydisplay/visual_table.png?raw=true)
