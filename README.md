## Experiment 19
## Aim:
To perform SET OPERATIONS on tables in MySQL.

## Algorithm:
1.Start MYSQL Workbench.

2.Create a database to store your data.

3.Use the database and create a table.

4.Inside the table ,create variables with appropriate datatype.

5.Insert values and apply logic to visualize the output.

## Program:
```
CREATE TABLE Speakers
(
  Name VARCHAR(25),
);

CREATE TABLE Authors
(
  Name VARCHAR(25),
);
INSERT INTO Speakers VALUES ('Sachin')
INSERT INTO Speakers VALUES ('Rahul')
INSERT INTO Speakers VALUES ('Kamplesh')
INSERT INTO Speakers VALUES ('Chirag')

INSERT INTO Authors VALUES ('Sachin')
INSERT INTO Authors VALUES ('Rahul')
INSERT INTO Authors VALUES ('Pratik')
INSERT INTO Authors VALUES ('Rajesh')
INSERT INTO Authors VALUES ('Anil')

----Union
select name from Speakers
union
select name from Authors
order by name
---union all
select name, 'Speaker' as 'Role' from Speakers
union all
select name, 'Author' as 'Role' from Authors
order by name
---intersect
select name from Speakers
intersect
select name from Authors
order by name
---except
select name from Speakers
except
select name from Authors
order by name
```
## Output 
![image](https://github.com/balaji-21005757/set-operations/assets/94372294/4e3b8603-2a76-44c9-8ba3-27332736293c)

## Result:
Therefore we have successfully performed SET OPERATIONS.
