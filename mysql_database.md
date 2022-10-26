1. Database creation command
Create Database student; // student =  Dataabase_Name

2. Table Creation Command
Create Table personal // personal = Table_Name
create table personal(
	id int,
    name varchar(50)
    birth_date varchar(20),
    gender varchar(10),
    phone int
);

3. Insert Data into Tables
insert into personal(id, name, birth_date, gender, phone) // personal == Table_Name
values (2, "Muhammad Ahmad Raza", "1997-01-01", "M", "123456789");

4. Insert Multiple Data into Table in single query 
insert into personal(id, name, birth_date, gender, phone) // personal == Table_Name
values 
(2, "Muhammad Ahmad Raza", "1997-01-01", "M", "123456789"),
(3, "Muhammad Ahmad Raza", "1997-01-01", "M", "123456789"),
(4, "Muhammad Ahmad Raza", "1997-01-01", "M", "123456789"),
(5, "Muhammad Ahmad Raza", "1997-01-01", "M", "123456789"),
(6, "Muhammad Ahmad Raza", "1997-01-01", "M", "123456789"),
(7, "Muhammad Ahmad Raza", "1997-01-01", "M", "123456789");

5. Using Constraints 
Create Table personal // personal = Table_Name
create table personal(
	id INT NOT NULL UNIQUE,
    name varchar(50) NOT NULL
    birth_date varchar(20) N0T NULL,
    age INT NOT NULL CHECK(age => 18)
    gender varchar(10),
    phone INT NOT NULL UNIQUE,
    city VARCHAR(20) DEFAULT "LAHORE"
);

6. To find out Data 
Select * from personal // personal = Table_Name // * == It means All Data
Select id, name, phone from personal // for specific column

6.1 Select with Where Clause
SELECT * FROM personal
WHERE gender = 'F'  // It shows only female data 
WHERE age < 24 // It shows only data who less than 24 ages

7. AND, OR, NOT Operators

SELECT * FROM personal
WHERE age < 20 AND gender="M";

SELECT * FROM personal
WHERE (age < 54 AND gender="M") AND city="Okara"; // Complex Condition 

8. IN Operator 

Select * from personal
Where id IN(1,2, 4) // Find multiple columns 

9. Between Operator 
use for find value using range 

10. Like Operator 
% Percentage Characters // Represent Zero, One, Multiple Characters
_ Underscorre Chractor // Represent Single Characters