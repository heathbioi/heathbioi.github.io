# Data transfer from WGP

 ## Connect to RDS from HAWK

 Go to terminal and insert:

  ```
ssh c.$USER@hawklogin.cf.ac.uk
(c.$USER@hawklogin.cf.ac.uk) Password: (yourHAWKpassword)
ssh rds
c.$USER@rds's password: (yourHAWKpassword)
access_rds.sh
My CU ID is: cxxxxx
Please enter your CU ID password to access the RDS (NOT SCW password):
Password: (yourRDSpassword)

  ```
 
Go to RDS
```
cd /rds/
ls
```
Check storage combined 
```
 du -sh
```
	
 Check storage Individual
 
```
	[c.c1460532@rds rds]$ du -sh *
	845G	137339876
	3.4T	220339937
	830G	69572051
	1.9T	87405545
	4.0K	README.txt
```
Choose directory to place data in and navigate to directory
```
cd directory/
ls
data analysis
```

Create new directory for data
```
mkdir pgdsXXXX
ls
 pgdsXXXX
 ```
go to new data directory

```
cd pgdsxxxx
```

Download data using link to fastq files
Use wget

Push data to HAWK
Copy data from rds into data.nextflow
[c.c1460532@rds 220339937]$ cp -r pgds0001 /scratch/c.c1460532/data.nextflow/

Record new data ID and location in README file

Perform analysis

