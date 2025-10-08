**Assignment 2: Database creation, deletion and OEM**

**Name:** UWAYO Nziza Ines.

**Student ID:** 27902.

  **OVERVIEW**
This assignment demonstrates how to create and delete pluggable databases(PDBs) and configure Oracle Enterprise Manager(OEM) Express in Oracle Database.

We were given 3 tasks:

  **Task 1:** **Create a New Pluggable Database**

The objective for this task was to create a new pluggable database to store all class work for this course.

The instructions were to create a database named FirstTwoLettersOfFirstName_pdb_StudentID, so I named my database: in_pdb_27902

And the username format was : FirstName_plsqlauca_StudentID
So my username was ines_plsqlauca_27902

First I logged in as sys user in SQLPLUS : 

As indicated in the screenshot in [Logging_in_as_sysdba.png](screenshots/Logging_in_as_sysdba.png)

Then I procceded by creating the Pluggable Database: [creating_1st_PDB.png](screenshots/creating_1st_PDB.png)

And then the PDB  was created: [show_PDB1_output.png](screenshots/show_PDB1_output.png)

  **Task 2:** **Create and Delete a PDB**

The Objective of this task was to create a temporary PDB and then delete it.

The format was :  FirstTwoLettersOfName_to_delete_pdb_StudentID

So i created a PDB named: in_to_delete_pdb_27902

I started by creating the database as shown in : [creating_to_delete_PDB.png](screenshots/creating_to_delete_PDB.png)

Then I got confirmation: [to_delete_PDB_created.png](screenshots/to_delete_PDB_created.png) 

Then I checked if the PDB had been created : [showing_to_delete_PDB.png](screenshots/showing_to_delete_PDB.png)

I proceded to delete the PDB : [to_delete_PDB_deleted.png](screenshots/to_delete_PDB_deleted.png)

Then I verified if the deletion was successful : [verifying_deletion.png](screenshots/verifying_deletion.png)

  **Task 3:** **Oracle Enterprise Manager**

The Objective of this task was to configure Oracle Enterprise Manager(OEM) Express for the Database and verify the dashboard.

Here is the configuraion of the Oracle Enterprise Manager : [configuring_OEM.png](screenshots/configuring_OEM.png)

Then I logged in as sys to check the dashboard.

Then I went to check the dashboard : [OEM_dashboard.png](screenshots/OEM_dashboard.png)

**Below are some challenges that I met and how I solved them**

The challenge I met is that at first the OEM was not opening in the browser. 

I came to an understanding that it was being 
caused by the fact that HTTPS port was not configured and so I set the port using DBMS_XDB_CONFIG.SETHTTPSPORT(5501).

  **Conclusion**

The assignment successfully demonstrated PDB creation, deletion, and configuration of Oracle Enterprise Manager (OEM) Express in Oracle Database.

All tasks were verified with screenshots and executed without errors.
