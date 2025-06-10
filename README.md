# my-termux-mariadb-analytics-journey

A documentation on how to be able to write SQL on Android phone or tablet with Termux and Mariadb.

## Installing Termux
Download Termux from **F DROID**

run: 
pgk update
pgk upgrade

## Installing Mariadb IN Termux
In Termux run:
pkg install mariadb       (mariadb is a RDBMS that is alternative for MySQL)

_ _after installation_ _
mysqld_safe &             (to start mariadb server) 

## setting a root password
run:
mysql -u root
ALTER USER 'root'@'localhost' IDENTIFIED BY 'your password';
FLUSH PRIVILEGES;
EXIT;

## If you already have a MYSQL server (maybe from other devices) you can connect it to Mariadb.
_ _after you installed mariadb_ _

run:
mysql -h your.mysql.server.ip -yourusername -p

enter your password when prompted


There you have it, you now have access to mysql on your tablet or android phone. You can practice your sql commands and run it in your phone even OFFLINE.


