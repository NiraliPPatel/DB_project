CS6360: Database Design

# Davisbase 

## Requirements
- Java 8
- Maven 3.6.x

## Installation 

>Linux - Debian Based
```
$ sudo apt install openjdk-8-jdk
$ sudo apt install maven
```
> For Other Operating Systems please refer [Apache Maven Installation.](https://maven.apache.org/install.html)

## Compilation and Execution
```
$ mvn clean package
$ java -cp target/classes edu.blue.Davisbase
```

## Supported Commands

```
help;
version;
show tables;
create table <table-name> (Column_Name DataType [unique] [primary key] [not null], [multiple...]);
create index on <table-name> (Column_Name);
insert into <table-name> (Column_Name, [Column_Name(s)...]) values (Value, [Values...]);
select * from <table-name> [where CONDITION];
update <table-name> set name=VAL where CONDITION;
drop table <table-name>;
```

## Commands for Reference

```
create table user (id int,name text);
insert into user (id,name) values (1,john);
select * from user;
update user set name = mark where id = 1;
select * from user where id=1;
create index on user (name);
delete from table user where id=1;
drop table user;

```

> **NOTE:** The application only supports single where clause in SELECT, UPDATE and DELETE operations



### Authored by Team Blue
- Chetan Garikapati (CXG190009)
- Prajjwal Bhargava (PXB190028)
- Jessica Su (JXS190058)
- Pengchao Cai (PXC190029)
- Nikhil Bollepalli (NXB200019)
