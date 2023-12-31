# InformativeDatabase
@author Matthew Kim
Date: 05/31/2023
Course: TCSS 445 A - Database System Design
Project: Final Project Submission


Forager Information System:
Preface: The purpose of this application is to be able to search specific forager's journal pages by entering a
         mushroom/ plant species and mushroom/ plant common names.


How-To-Use-This-Application:
1) Load 'Kim_Matthew_QUERIES.sql' into SQL Server Manager Studio
    - Execute Statements:
       - Create Database ...
       - USE ...
       - CREATE (all Tables)...
       - INSERT (all data)...

2) Open 'Kim_Matthew_Forager_Information_System...' project folder in IntelliJ IDEA or Ultimate IDE

3) Some setting have to be changed to be able to make the files work right
     - Go to File tab -> Project Structure -> Modules
     - add (+) jar file -> mssql-jdbc-12.2.0.jre11.jar   *Included in Zip folder in src folder
     - change 'Module SDK' -> 19 Oracle OpenJDK version 19.0.2
     - Apply -> Ok

4) Open LoadData.java Class and go to lines 18-21:
     - Need to reconfigure SQL server settings to your computer
     -     private String serverName = "...Server Name...";
           private String databaseName = "...Database Name...";
           private String username = "...Login...";
           private String password = "...Password...";

5) Open ForagerApplication.java Class and go to line 41
    - Run main() to start the GUI application

6) Once the GUI opens you will see a 'Menu' section on the left and a 'Journal Page' section on the right
    - In Menu:
      - Select a username i.e. "Test1"
      - Click 'Load Forager Database' button, This will populate data either in the 'Mushroom Forager Database' or
        the 'Plant Forager Database' section of the 'Menu'.
      - Depending on the username's journal page entries CLICK either the 'Mushroom Journal Page Search' button or
        'Plant Journal Page Search' button (If mushroom species or common name is empty in the comboBox then
        do not click that search button)

7) Once a search (query) to the database has been commenced, the Journal Page (right side of the application) will
   populate with data for that specific mushroom journal page or plant journal page.

8) You can repeat step 6 with a different username and load that part of the database in there to utilize the application
   further.


