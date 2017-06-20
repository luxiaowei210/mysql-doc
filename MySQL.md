# MySQL的安装

# 创建数据库 

 create database stu;

# 创建表

```mysql
create table school(
sno int not null primary key, 
sname char(20) not null)character set = utf8;
create table information(
id int not null primary key, name varchar(20) not null, 
age int not null, sex varchar(10) not null, 
sno int not null)character set = utf8;
create table score(
num int not null primary key, score int(20) not null, 
id int not null)character set = utf8;

select *from school
select *from information
select *from score

drop table school
drop table information
drop table score

insert into school(sno , sname ) value (41 , '软件')

create database stu;
create table school(
sno int not null primary key, 
sname char(20) not null)character set = utf8;
create table information(
id int not null primary key, name varchar(20) not null, 
age int not null, sex varchar(10) not null, 
sno int not null, foreign key (sno) references school(sno) )character set = utf8;
create table score(
num int not null primary key, score int(20) not null, 
id int not null, foreign key (id) references school(id))character set = utf8;
```
