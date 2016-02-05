# Tornado Blog
Quick &amp; simple blog using the Tornado framework

## Getting started

- Install Tornado @ http://www.tornadoweb.org/

- Install & launch MySQL
```bash
brew install mysql
```
or
```bash
pip install mysql
```
- Connect to MySql

```bash
mysql -u root
mysql> CREATE DATABASE blog;
mysql> GRANT ALL PRIVILEGES ON blog.* TO 'blog'@'localhost' IDENTIFIED BY 'blog';
```
- Create the tables in your MySQL database
```bash
mysql --user=blog --password=blog --database=blog < schema.sql
```
- Start your blog
```bash
./blog.py
```
or 
```bash
python blog.py
```
Should start running on localhost:8888
