
```
create database diu;

-- create table
CREATE TABLE students (
    id INT PRIMARY KEY AUTO_INCREMENT,
    name VARCHAR(200),
    dob DATE
);

insert into students(name,dob)
values
("HR Utsha","2000-12-20"),
("Rashid","2001-12-27");

SELECT 
    *
FROM
    students;


/* table modification
1. add new column 
2. modify column data types
3. modify column name 
4. drop column
5. rename table
6. truncate
7. drop table 
*/

-- 1. add a new column
alter table students add gmail varchar(100);
alter table students add phone int;

-- 2. modify column data types
alter table students modify name varchar(300);

-- 3. modify column name 
alter table students rename column name to full_name;
alter table students rename column full_name to `full name`;

-- 4. drop column
alter table students drop column gmail;
alter table students drop column phone;

-- 5. rename table
rename table students to learners;

-- 6. truncate
truncate table learners ;

-- 7. drop table 
drop table learners;






```
