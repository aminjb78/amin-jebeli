# amin-jebeli
مباحث تدریس شده استاد عدل دوست / کلاس ساعت 11 / یکشنبه

select * from person;
select * from studebt;
select count(*), mobile from person group by mobile;
select max(*),city from person group by mobile;
select count(id),city from person group by city having(id)>2;

select sum(id) from person;
select replace(first_name,'amin')from person;
selecr * from person where id>=3 and id<=7;
selecr * from person where id between 3 and 7;
selecr * from person order by national_code asc;
selecr * from person where first_name like;
update person set mobile=null where id =8;
select top 3 * from person order by id desc;
SELECT Orders.OrderID, Customers.CustomerName, Orders.OrderDate
FROM Orders
INNER JOIN Customers ON Orders.CustomerID=Customers.CustomerID;

SELECT COUNT(CustomerID), Country
FROM Customers
GROUP BY Country
ORDER BY COUNT(CustomerID) DESC;


select p.id as p.first_name as p.last_name,s.student_number from person p left join student s on p.id=s.person_id;
select * from person,student where person.id=student.person_id;
insert inti major(title,description)values('hesabdari','bababababa');
insert into student(person_id,student_number,edu_level,major_id)values(3,96124,1,null);
update student set major_id=1;
select * from student left join major on student.major_id=major.id union all;
select * from student rightjoin major on student.major_id=major.id where major_id is null;


insert into student(person_id,student_number,edu_level,major_id)values(2,111,1,1);
insert into person (first_name,last_name,national_code,mobile)values('tes4'),('test3'),(''test2'),('test1');
update person set mobile=concat('first_name')where first_name='amin'or national_code='0001';
delete from person where id =4;
