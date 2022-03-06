![Screenshot](resource/phpadminmysql.png)
# Install software
```bash
git clone https://github.com/sonnyyu/docker-phpmyadmin/
cd docker-phpmyadmin
```
# Getting started
```bash
docker-compose up -d
```
# Quit and remove volume
```bash
docker-compose down  -v
```

# Open web interface
https://ip:8086/    admin:admin

# Create DB, User and grant access 
```bash
CREATE DATABASE wordpress;
CREATE USER 'wordpress'@'%' IDENTIFIED BY 'wordpress';
GRANT ALL ON wordpress.* TO 'wordpress'@'%';
FLUSH PRIVILEGES;
```
