# Tornado Blog
Quick &amp; simple blog using the Tornado framework

## Getting started

1. Install Tornado @ http://www.tornadoweb.org/

2. Install & launch MySQL
` brew install mysql ` or `pip install mysql`

3. Connect to MySql
```bash
mysql -u root
mysql> CREATE DATABASE blog;
mysql> GRANT ALL PRIVILEGES ON blog.* TO 'blog'@'localhost' IDENTIFIED BY 'blog';
```
4. Create the tables in your MySQL database
```bash
mysql --user=blog --password=blog --database=blog < schema.sql
```
5. Start your blog
```bash
./blog.py
```
or 
```bash
python blog.py
```
Your blog is running on localhost:8888
