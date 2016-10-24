Instalation of ims system guide Created By 8ex0r

1) MySQL Database server running on localhost user:root , pass: root1

2) Create database ims1;   (don't confuse with ims1-database name, ims2- project name)

3) Create table Name : mailusers using following query ..
   
    Create table mailusers(uname varchar(10) not null, pwd varchar(10) not null,age int(3), sex varchar(10), city varchar(10), state varchar(10), pincode int(6), nation varchar(10));
    
4) this project devloped under web module version 2.5  (Apache Tomcat 7.0) 

5) add and run project in apache tomcat 7



used tools for compiling and Running project ims2
1) eclipse-jee-luna-R-win32 (web module version 2.5) 
2) apache-tomcat-7.0.68 
3) java version "1.8.0_60"
4) MySQL Server version: 5.7.11 


Mysql root Password Change
login in mysql console as root

mysql> use mysql;
mysql> update user set password=PASSWORD("root1") where User='root';
mysql> flush privileges;
mysql> quit
