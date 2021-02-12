INSERT into cars value (DEFAULT, 'BMW');  # default = id
INSERT into cars value (DEFAULT, DEFAULT);

SELECT * FROM students;
SELECT name, age FROM students;

SELECT * FROM students WHERE age = 15;
select * from students where name = 'roman';
select * from students where name = 'RoMaN';

select * from students where name like '%n';
select * from students where name like 'o%';
select * from students where name like '%n%';
select * from students where name like '___a%';

select * from students where length(name) = 4;

select * from students where name like 'o%' order by age desc;
select * from students where name like 'o%' order by age asc;
select * from students order by age desc;
select * from students order by age asc;

select * from students where age != 20;
select * from students where age <> 20; # аналогічно як попередній оператор

select * from students where age > 20;
select * from students where age < 20;

select * from students where age between  20 and 30;
select * from students where age > 20 and age < 30;

select * from students where age > 19 and name like 'o%'; # wildcard

select * from students where age = 18 or gender = 'female' and name like 'o%';

select * from students where age = 20 or age = 35;
select * from students where age in(20, 25, 30, 35);

# Aggregate functions
select max(age) as MaxAge from  students;
select min(age) as MinAge from  students;
select avg(age) as AvgAge from  students;

select count(id) from students;
select count(id) from students where age > 50;

select sum(age) from students;

select * from students where age = (select max(age) from students); # multiselect

# Limit and Offset
select
       avg(rating) as AvgRating,
       count(rating) as Count
from ratings where student_id = 5;

select * from students order by age limit 3;
select * from students order by age limit 3 offset 6; # 3 студента після перших 6 студентів


# Set and Delete

update students set name = 'Valentin', gender = 'chubaka' where age = 20;
update students set name = 'Moroz' where age = 25;
update students set age = 20 where age > 40;

delete from students where gender = 'chubaka';

