

create table Age (
ageId number primary key, 
age number 
);

create table Office (
officeId number primary key, 
office varchar(20) 
);

create table Salary(
salaryId number primary key,
salary number
);

create table Employee (
idEmp number primary key, 
nameEmp varchar(20), 
ageId number, 
officeId number, 
salaryId number,
constraint employee_age foreign key(ageId) references Age(ageId),
constraint employee_office foreign key(officeId) references Office(officeId),
constraint employee_salary foreign key(salaryId) references Salary(salaryId) 
);

insert into Age values (1, 18);
insert into Age values (2, 19);
insert into Age values (3, 20);

insert into Office values (1, '28 may');
insert into Office values (2, 'Sahil');
insert into Office values (3, 'Iceri sheher');

insert into Salary values (1, 1000);
insert into Salary values (2, 2000);
insert into Salary values (3, 3000);

insert into Employee values (1, 'Murad', 1, 2, 1);
insert into Employee values (3, 'Tural', 3, 3, 2);
insert into Employee values (2, 'Leman', 1, 2, 1);

select * from Age ;

select * from Office ;

select * from Salary ;

select * from Employee ;

select * from Employee 
join Age on Employee.ageId = Age.ageId
join Office on Employee.officeId = Office.officeId
join Salary on Employee.salaryId = Salary.salaryId ;


drop table Employee; 

create table Employee (
idEmp number primary key, 
nameEmp varchar(20), 
ageId number, 
officeId number, 
salaryId number,
constraint employee_age foreign key(ageId) references Age(ageId) on delete cascade,
constraint employee_office foreign key(officeId) references Office(officeId) on delete cascade,
constraint employee_salary foreign key(salaryId) references Salary(salaryId) on delete cascade 
);

insert into Employee values (1, 'Murad', 1, 2, 1);
insert into Employee values (3, 'Tural', 3, 3, 2);
insert into Employee values (2, 'Leman', 1, 2, 1);

select * from Employee 
join Age on Employee.ageId = Age.ageId
join Office on Employee.officeId = Office.officeId
join Salary on Employee.salaryId = Salary.salaryId ;


drop table Employee; 

create table Employee (
idEmp number primary key, 
nameEmp varchar(20), 
ageId number, 
officeId number, 
salaryId number,
constraint employee_age foreign key(ageId) references Age(ageId) on delete set null,
constraint employee_office foreign key(officeId) references Office(officeId) on delete set null,
constraint employee_salary foreign key(salaryId) references Salary(salaryId) on delete set null 
);

insert into Employee values (1, 'Murad', 1, 2, 1);
insert into Employee values (3, 'Tural', 3, 3, 2);
insert into Employee values (2, 'Leman', 1, 2, 1);

select * from Employee 
join Age on Employee.ageId = Age.ageId
join Office on Employee.officeId = Office.officeId
join Salary on Employee.salaryId = Salary.salaryId ;

