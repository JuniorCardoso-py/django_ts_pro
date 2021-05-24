# django_ts_pro



## Description

<p align="center"> This is a simple aplication to train the knowledges with docker-compose and django </p>


<img src="https://img.shields.io/static/v1?label=Django&message=Django_APP&color=#44B78B&style=for-the-badge&logo=ghost"/>

<p align="center">
 • <a href="#objetivo">Run an app django with docker-compose</a></br> •
 <a href="#tecnologias">Django, Python, Postgres, Docker</a></br> • 
 <a href="#licenc-a">MIT</a></br> • 
 <a href="#autor">Junior Cardoso</a></br>
</p>

### Pré-requisitos

Antes de começar, você vai precisar ter instalado em sua máquina as seguintes ferramentas:
[Git](https://git-scm.com),
[Python 3.9^](https://www.python.org/downloads/), 
[Docker](https://docs.docker.com/docker-for-windows/install/). 
Além disto é bom ter um editor para trabalhar com o código como [VSCode](https://code.visualstudio.com/)

### 🎲 Rodando o Back End (servidor)

```bash
# Clone este repositório
$ git clone <https://github.com/JuniorCardoso-py/django_ts_pro.git>

# Acesse a pasta do projeto no terminal/cmd
$ cd django_ts_pro

# With poetry installed on your SO, run the following commands
$ poetry shell
$ poetry install

# Next run the DataBase docker container on cmd/terminal
$ docker-compose up --build -d

# You may need to run the migrations
$ python manage.py migrate

# You will need to create an user and an password to access the admin site
$ python manage.py createsuperuser

# The server will start on port:8000 access <http://localhost:8000/admin>
$ python manage.py runserver

```