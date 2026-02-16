Oracle Pluggable Database Administration Assignment

Student Information
Name: Kirenga Fabrice
Student ID: 28367
Date: February 16, 2026

Oracle Environment
Oracle Version: Oracle Database 21c Enterprise Edition
Operating System: Microsoft Windows x64
CDB Name: ORCL
PDB Created: KR_PDB_28367

Task 1: Create a New Pluggable Database
PDB Name: kr_pdb_28367
Username Created: KIRENGAFABRICE_PLSQLAUCA_28367
Password: auca1

Steps Performed:

Connected as SYSDBA to CDB$ROOT

Created PDB using FILE_NAME_CONVERT with path C:\ORACLEE21C\ORADATA\ORCL\

Opened the PDB with ALTER PLUGGABLE DATABASE OPEN

Verified PDB status using v$pdbs

Granted CONNECT, RESOURCE, and CREATE SESSION privileges

Screenshots:
PDB Creation
PDB Open State
User Verification

Task 2: Create and Delete a Temporary PDB
Temporary PDB Name: kr_to_delete_pdb_28367

Steps Performed:

Created temporary PDB using same file path pattern

Opened the PDB and verified both PDBs existed

Closed and dropped the temporary PDB with INCLUDING DATAFILES

Confirmed deletion by querying v$pdbs

Screenshots:
Temporary PDB Creation
Both PDBs Visible
Deletion Command
Final Verification

Task 3: Oracle Enterprise Manager (OEM)
EM Express Port: 5501
Access URL: https://localhost:5501/em

Steps Performed:

Configured EM Express port using DBMS_XDB_CONFIG.SETHTTPSPORT(5501)

Successfully logged in as KIRENGAFABRICE_PLSQLAUCA_28367

Dashboard shows PDB KR_PDB_28367

Screenshots:
OEM Dashboard

Challenges Faced and Solutions

Challenge	Solution
ORA-65005: File path error	Corrected path from C:\ORACLEE21\ to C:\ORACLEE21C\
ORA-01920: User name conflict	Used uppercase username KIRENGAFABRICE_PLSQLAUCA_28367
ORA-12154: TNS could not resolve identifier	Used EZCONNECT format: localhost:1521/kr_pdb_28367
ORA-31050: EM Express access denied	Configured port 5501 and granted proper privileges
Integrity Statement
I hereby declare that this assignment is my own work and follows all naming conventions as specified in the assignment brief. All screenshots are authentic and taken from my own Oracle environment.


Date: February 16, 2026


