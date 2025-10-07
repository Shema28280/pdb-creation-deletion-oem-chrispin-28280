# Oracle Pluggable Database Administration: Creation, Deletion, and Performance Monitoring

* Course: Database Development with PL/SQL (INSY 8311)

* Instructor: Eric Maniraguha

* Student Name: NTAMBARA SHEMA CHRISPIN

* Student_ID: 28280


# Summary

* There are two stages of creating, managing, and deleting a Pluggable Database (PDB) in Oracle Database 21c XE, which are documented in this project.  
* It is also associated with the monitoring of the PDB using the Oracle Enterprise Manager (OEM) and the troubleshooting of the common problems involved with the process.


# Tasks Performed

1. Create a Pluggable Database (PDB) 

2. Access and verify the PDB through Oracle Enterprise Manager (OEM).

3. Delete the created PDB and verify removal.  

4. Document issues and resolutions encountered during each step.


# Screenshots

1. PDB Creation: Successful creation message in SQL Plus.
(<PDB Creation Successful creation message in SQLPlus..png>)

2. OEM Dashboard: PDB visible and active. 
(<OEM Dashboard.PNG>)


3. PDB Creation & Deletion: Creation & Drop confirmation message. 
(<PDB Creation.PNG> & <PDB Deletion.PNG>)


# Challenges & solutions

During this database administration assignment, I went through a number of challenges.

* The first was the error of ORA-65118 that was caused due to the fact that the container database (CDB) was in the read-only mode. I resolved this by putting the CDB in read- write mode before trying to create the pluggable database (PDB). 

* The other problem was that I did not see my PDB visible in Oracle Enterprise Manager (OEM) once created. This occurred due to the failure to refresh the listener or OEM service. I resolved to restart the listener and refresh OEM, after which the new PDB was displayed successfully on the dashboard.

* Also, the OEM performance dashboard displayed the message of No data to display. This is because it had not gone through any recent database activity, i failed to solve this.

* Lastly, I had attempted to drop the to-delete PDB by using the DROP PLUGGABLE DATABASE command, and it failed to work at first since there were active sessions attached to it. I decided this by shutting down all the open connections and re-executing the drop command.

