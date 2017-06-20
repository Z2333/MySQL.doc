# MySQL.doc
6月15 星期四
## 安装数据库（sudo apt-get update 更新源
sudo apt-get install mysql-client mysql-server 安装mysql服务器和客户端）
## 安装Apache（sudo apt-get update（因为之前进行了更新源所以这一步不用再做）
sudo apt-get install tasksel）
## 安装mysql-workbench（sudo apt-get install mysql-workbench）
## 建立数据库stu (create database stu)
## 进入数据库（ mysql -u root -p）
## 显示数据库（show databases）
## 创建数据表 school（ create table 
数据|英文名|数据类型|备注
-----|-----|-----|-----
学校名|Sname|char(20)| not null|
学校地址|address|char(20)| not null|
学校编号|Sid|not null|primary key auto_increment主码|
## 创建数据表 information（create table information）
数据|英文名|数据类型|备注
-----|-----|-----|-----
学生姓名|name| char(20)| not null|
学生性别|sex| int(4)| not null default '0'|
学生编号|id| int(4)| not null|
主码， 外码是学校编号（Sid）
## 创建数据表 score（create table score）
数据|英文名|数据类型|备注
-----|-----|-----|-----
课程编号|id|char(20)|
课程名|course| char(20)| 
成绩|score|int| 
外码：课程编号（id）和课程名（course）
