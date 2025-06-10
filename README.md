# my-termux-mariadb-analytics-journey

A documentation on how to be able to write SQL on Android phone or tablet with Termux and Mariadb.

---

## What is Termux? ##

## What is Mariadb? ##

---

## Installing Termux
Download Termux from **F DROID**

run: 
pkg update
pkg upgrade

---

## Installing Mariadb IN Termux
In Termux, run:
``` bash
pkg install mariadb
```
_after installation_

To start mariadb server
```bash
mysqld_safe &
```
---

## setting a root password, run:
```sql
mysql -u root
ALTER USER 'root'@'localhost' IDENTIFIED BY 'your password';
FLUSH PRIVILEGES;
EXIT;
```


## If you already have a MYSQL server (maybe from other devices) you can connect it to Mariadb.
_after you installed mariadb_

run:
mysql -h your.mysql.server.ip -yourusername -p

enter your password when prompted


There you have it, you now have access to mysql on your tablet or android phone. You can practice your sql commands and run it in your phone even OFFLINE.


