# os-db-json-tester
Scripts to test out JSON functionality in MySQL, PostgreSQL, and MongoDB... and simulate generate load

##  For Testing MySQL:

### Step 1

create database using MySQL/mysql_json_create_tables.sql (Change the password for the user created to what you want )

 ```bash
mysql -uroot -p
mysql> source MySQL/mysql_json_create_tables.sql;

 ```

### Step 2
Get your data from movienet.site, ( you need to register in the site to download the package)
https://opendatalab.com/MovieNet/download
Look for meta and then unpack meta.v1.zip into the meta/ directory.

### Step 3
Update passwords in scripts under MySQL/* as needed, ensure python is setup along with the mysql connector


### Step 4
Run "python3 mysql_load_tables.py"