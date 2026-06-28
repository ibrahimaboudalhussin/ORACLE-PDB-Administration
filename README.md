 Assignment II: Oracle Pluggable Database (PDB) Administration

**Student Name:** Ibrahim  
**Student ID:** 32070  
**Course:** Advanced Database Systems / PL-SQL Administration  
**Date:** June 28, 2026

 Executive Summary
This report documents the successful completion of Assignment II regarding Oracle 19c/21c Pluggable Database (PDB) Administration. The tasks achieved include creating a dedicated production PDB, managing its states, provisioning a new localized administrative user with granular privileges, verifying cross-container connectivity, and implementing a strict lifecycle test by creating and dropping a temporary PDB.


 Task 1: Permanent PDB Creation and User Provisioning

Step 1: Creating the Permanent PDB
A permanent Pluggable Database named `ib_pdb_32070` was successfully created from the reference seed database container.

```sql
CREATE PLUGGABLE DATABASE ib_pdb_32070 
ADMIN USER pdbadmin IDENTIFIED BY Ibrahim2026 
FILE_NAME_CONVERT=('pdbseed', 'ib_pdb_32070');
