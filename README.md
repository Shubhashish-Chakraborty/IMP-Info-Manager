# IMP-Info-Manager

This project is for my ALL ACCOUNTS Management purpose. <br>

The concept of the project is: <br>

I can store my mail accounts , social media accounts there passwords and lots and lots of things
which i am working on...and will Keep updating the code further 


<hr>


HOW TO USE and ACCESS THE PROJECT: <br>


First of all create a database on your system named -> important_shubhdata (OR ANYTHING AS YOU WISH)<br>

BUT MAKE SURE while performing connection, mention your DATABASE EXACT NAME <br>
in here:

```python
myConnection = mysqlconnector.connect(host='localhost',user='root',passwd=MYpasswd database='<your-database>')
```

Then Create the required tables which is being mentioned below: <br>


# Copy the MySQL code from the below provided links to create the necessary tables.

sql query for gmailacc:
```bash
create table gmailacc(
    Sno integer(3) primary key,
    Gmail_Account varchar(50) not null,
    Password varchar(80),
    Extra_info varchar(80)
);
```
sql query for socialmediaacc:
```bash
create table socialmediaacc(
    Sno integer(3) primary key,
    Social_Account varchar(50) not null,
    Password varchar(80),
Extra_info varchar(80)
);
```
sql query for otheracc:
```bash
create table otheracc(
    Sno integer(3) primary key,
    Account_Name varchar(80) not null,
    Password varchar(80),
    Extra_info varchar(80)
);
```
sql query for contactdetails:
```bash
create table contactdetails(
    Sno integer(3) primary key,
    Contact_Name varchar(50) not null,
    Contact_Number varchar(80),
    Extra_info varchar(80)
);
```