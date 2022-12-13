# Cinema API
API service for a cinema. Written in Python using Django REST Framework.
### Installation
Install PostgresSQL and create db

Clone repository `git clone https://github.com/wQuelS/cinema-api.git`  
Change directory `cd cinema-api`  
Set environment `python -m venv venv` and activate it `source venv/bin/activate`  
Install all requirements via `pip install -r requirements.txt`  
 Now you can set variables for DB and migrate:  
```
DB_HOST=<your db hostname>
DB_NAME=<your db name>
DB_USER=<your db username>
DB_PASSWORD=<your db user password>
SECRET_KEY=<your secret key>
python manage.py migrate
python manage.py runserver
```


### Run Docker containers
Docker should be installed
```
docker-compose build
docker-compose up
```
### Getting access
Domain: `127.0.0.1:8000`

Create user: `/api/user/register/`  
Get JWT Token: `/api/user/token/`

### Features
* JWT authenticated
* Admin panel
* Swagger documentation is located at /api/doc/swagger/
* Managing orders and tickets
* Creating cinema halls
* Creating movies with genres, actors
* Adding movie sessions
* Filtering movies and movie sessions
* Postgres database
