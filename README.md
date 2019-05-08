# Egg-todos

# 启动

## 数据库下载安装
[MySQL下载地址](https://dev.mysql.com/downloads/)
1. 安装完成后，开启mysql服务，设置密码：
```bash
mysql -u root -p // 输入安装结束时设置的密码，如111111
```
2.  新建数据表
```sql
create database test DEFAULT CHARSET utf8 COLLATE utf8_general_ci;
use test;
create table todoList(
  id int auto_increment primary key, 
  title char(30) not null,
  completed TINYINT(1) DEFAULT 0;
);
```

## 启动后台服务

```bash
$ npm install
$ npm run dev
```

## 启动前台页面

```bash
$ npm install
$ hey dev
```