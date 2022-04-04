---
layout: default
title: Query to Display Data
nav_order: 5
---

# Query to Modify Data
For this section we will be displaying a table from the database in MySQL Workbench. 

This tutorial works with the table used in [Query to Modify Data](modify) and also works with any tables on MySQL in general.

A visual representation of a table in MySQL will look like the following figure.

  ![MySQL Workbench visual table](https://github.com/dvalle22/Mel-Danilo-Cody/blob/gh-pages/assets/images/querydisplay/table_intro.png?raw=true)

As shown in the figure above, the column names are listed at the top followed by every row of student information inserted into the table.

Follow the steps below to acheive this.

1. In MySQL Workbench, click the 'Create a new SQL tab for executing queries' icon at the top left corner of the window as shown below. 
    ![MySQL Workbench new SQL query tab](https://github.com/dvalle22/Mel-Danilo-Cody/blob/gh-pages/assets/images/querydisplay/createsql_tab.png?raw=true)

    A blank text file should appear in the centre pane of MySQL Workbench.
    
    ![MySQL Workbench blank text file](https://github.com/dvalle22/Mel-Danilo-Cody/blob/gh-pages/assets/images/querydisplay/blank_textfile.png?raw=true)
<br />
2. Copy the block of code below
      ```sql
    SELECT *
    FROM user;
    ```

<br />
3. Paste the copied code into the blank text file. 
    
    ![MySQL Workbench code pasted to query file](https://github.com/dvalle22/Mel-Danilo-Cody/blob/gh-pages/assets/images/querydisplay/select_all_pasted.png?raw=true)
    
    The * here can be thought of the word 'all'.
    
    If you are using a different table you can replace _user_ from the copied code from Step 2.
    
    ![MySQL Workbench code pasted to query file different table name](https://github.com/dvalle22/Mel-Danilo-Cody/blob/gh-pages/assets/images/querydisplay/own_table.png?raw=true)
    
<br />
4. Click on the execute icon

    ![MySQL Workbench execute tab](https://github.com/dvalle22/Mel-Danilo-Cody/blob/gh-pages/assets/images/querydisplay/execute.png?raw=true)
    
<br />
5. View the table in the centre pane. 

    ![MySQL Workbench table is now visible](https://github.com/dvalle22/Mel-Danilo-Cody/blob/gh-pages/assets/images/querydisplay/table_appears.png?raw=true)
    
    Depending on your window size, you may need to hover your mouse over any of the four sides of the pane to readjust its size.
    
<br />



