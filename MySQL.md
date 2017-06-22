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
create table teacher(tid varchar(20) not null primary key, tpassword varchar(20) not null);
  create table student(id varchar(32) not null primary key, spassword varchar(32) not null);
```
# 基本命令
* 1.连接数据库命令 mysql -u root –p 回车后提示你输密码.注意用户名前可以有空格也可以没有空格
* 2. 连接到远程主机上的MYSQL命令  mysql -h110.110.110.110 -u root -p 123;（root为用户名 123为密码）
* 3. exit 退出数据库
* 4. create database <数据库名>  （创建数据库）
* 5. show databases； 显示数据库
* 6. drop database <数据库名>  删除数据库
* 7. use <数据库名> 使用数据库
* 8. select database(); 输出相关信息
* 9. create table <表名> ( <字段名1> <类型1> [,..<字段名n> <类型n>]); 创建表
* 10. drop table <表名> 删除表
* 11. insert into <表名> [( <字段名1>[,..<字段名n > ])] values ( 值1 )[, ( 值n )] 向表中插入数据
* 12. select <字段1，字段2，...> from < 表名 > where < 表达式 > 查询表中数据
* 13. update 表名 set 字段=新值,... where 条件 修改表中数据
* 14. alter table 表名 add字段 类型 其他; 增加字段
* 15. alter table 表名 add index 索引名 (字段名1[，字段名2 ...]); 添加索引操作
* 16. show index from 表名 显示索引
* 17. alter table 表名 drop index 索引名; 删除索引

