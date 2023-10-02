卸载
rm -rf /etc/mysql/ /var/lib/mysql
apt autoremove 
apt autoclean

安装
apt-get install mysql-server -y
apt install mysql-client -y


密码修改
flush privileges;
alter user 'root'@'localhost' identified  with  mysql_native_password by '？？？'
update user set host='%' where user='root'


create database kaoshi default character set utf8mb4 collate utf8mb4_unicode_ci;
