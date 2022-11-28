# Cinema API
API service for a cinema. Written in Python using Django REST Framework.
### Installation
Install PostgresSQL and create db

```
git clone 
git clone https://github.com/IvanStored/cinema-api-docker.git
cd cinema-api-docker
python -m venv venv
source venv/bin/activate
pip install -r requirements.txt
set DB_HOST=<your db hostname>
set DB_NAME=<your db name>
set DB_USER=<your db username>
set DB_PASSWORD=<your db user password>
set SECRET_KEY=<your secret key>
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
