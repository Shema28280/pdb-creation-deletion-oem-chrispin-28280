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
   
<img width="673" height="551" alt="PDB Creation Successful creation message in SQLPlus" src="https://github.com/user-attachments/assets/85128b11-83ff-4102-b518-e6e85def8ddd" />

2. OEM Dashboard: PDB visible and active.
    
<img width="1342" height="276" alt="OEM Dashboard" src="https://github.com/user-attachments/assets/62b1f923-a80e-452f-8385-de93884aea79" />

3. PDB Creation & Deletion: Creation & Drop confirmation message.

<img width="615" height="451" alt="PDB Creation" src="https://github.com/user-attachments/assets/1ed6ef77-6fac-4af8-8cb3-707e589c6d4c" /> 

<img width="584" height="136" alt="PDB Deletion" src="https://github.com/user-attachments/assets/814179e8-33cf-4fbd-917d-135a4c1e83a4" />



# Challenges & solutions

During this database administration assignment, I went through a number of challenges.

* The first was the error of ORA-65118 that was caused due to the fact that the container database (CDB) was in the read-only mode. I resolved this by putting the CDB in read- write mode before trying to create the pluggable database (PDB). 

* The other problem was that I did not see my PDB visible in Oracle Enterprise Manager (OEM) once created. This occurred due to the failure to refresh the listener or OEM service. I resolved to restart the listener and refresh OEM, after which the new PDB was displayed successfully on the dashboard.

* Also, the OEM performance dashboard displayed the message of No data to display. This is because it had not gone through any recent database activity, i failed to solve this.

* Lastly, I had attempted to drop the to-delete PDB by using the DROP PLUGGABLE DATABASE command, and it failed to work at first since there were active sessions attached to it. I decided this by shutting down all the open connections and re-executing the drop command.

