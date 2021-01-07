### Sample data added to postges

```
testdata=# CREATE ROLE admin WITH LOGIN PASSWORD 'admin';
ERROR:  role "admin" already exists
testdata=# \c testdata admin
Password for user admin: 
You are now connected to database "testdata" as user "admin".
testdata=# CREATE TABLE data (ID SERIAL PRIMARY KEY, firstname TEXT, lastname TEXT);
CREATE TABLE
testdata=# INSERT INTO data (firstname, lastname) VALUES ('John', 'Doe');
INSERT 0 1
testdata=# exit
root@acbbebbe258c:/# exit
exit


```