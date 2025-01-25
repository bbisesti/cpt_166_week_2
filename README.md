# CPT 166 Introduction

## Welcome


Welcome to CPT 166!  This week we will be completing the following:

- Introducing PostgreSQL
- Creating a Database on your server
- Creating a simple table with one record in your database

## Introduction

### Introducing Data

Please read the following:

- [W3Schools PostgreSQL](https://www.w3schools.com/postgresql/)

  This website will give you an overview of what PostgreSQL is. Please read from the Tutorial PostgreSQL Home all the way through (and completing) create demo database. 
  
- [Allowing Remote Access](https://stackoverflow.com/questions/18580066/how-to-allow-remote-access-to-postgresql-database)

  This is a good overview of how you allow "remote access" (i.e. access from another server) onto your machine.  Please update the postgresql.conf file with the listen_addresses.  For pg_hba.conf please enter the following:

  host  postgres  test_account  192.168.2.51/24  md5

  This will allow a script I have running on my computer the ability to connect!  Once it successfully connects and runs a query your assignment for the week is complete!

- [Creating Role](https://www.geeksforgeeks.org/postgresql-create-role/)

  The above pg_hba.conf will not work unless you crewate the role in the database!  Please read this link on how to create roles in Postgres.  Then please create a role which can login with the password 'test_account_password' (not at all secure but when this assignment is done we will be wiping these accounts!
