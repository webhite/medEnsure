# Django Project

A web application built with **Django 6.0.1** and **Python 3.13.3**.

---

## 🚀 Tech Stack

- **Python:** 3.13.3  
- **Django:** 6.0.1  
- **Database:** MySql
- **OS:** Cross-platform (Linux / macOS / Windows)

---

## 📦 Requirements

Make sure you have the following installed:

- Python **3.13.3**
- pip (comes with Python)
- python -m venv env

Check versions:
```bash
python --version
django-admin --version
```
## DataBase SetUp
- install mysql-server
```bash
sudo apt install mysql-server
```
- start the service
```bash
sudo systemctl start mysql
```
- login to mysql
```bash
sudo mysql -u root
```
- create new database
```bash
mysql> create database <database name>;
```
- create new user
```bash
mysql> create user <username> identified by <password>;
```
- grant privileges to user
```bash
mysql> grant all privileges on <database name>.* to '<username>'@'locahost';
```
- quit mysql console
```bash
exit
```
- create local_settings.py file inside project folder
```bash
touch med_ensure/local_settings.py
```
- enter the below settings in local_settings.py
DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.mysql',
        'NAME': "<database-name>",
        'HOST':"localhost",
        'USER':"<username>",
        'PASSWORD': "<password>"
    }
}

