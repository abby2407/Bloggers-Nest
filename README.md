# Bloggers Nest

Bloggers Nest is a microblogging web application developed using python and flask framework where user can share their thoughts and opinions on any topics.
This project was developed by me as a part of leaning python and flask web framework.

## Getting Started

These instructions will get you a copy of the project up and running on your local computer for development and testing purposes. See deployment notes on how to deploy the project on a your system.

### Prerequisites

The necessary packages that needs to installed on your local machine for running this application are listed in the requirements.txt file and instructions on how to install them are given below.

```
requirements.txt
```

### Installing

Clone this repo to your local machine 

```
https://github.com/abby2407/Bloggers-Nest.git
```
                    or

Download the Zip file and extract it, then in the projects root folder, open terminal and execute these commands -:

```
pip3 install -r requirements.txt
```

## Necessary changes that need to be made before running the application

open config.py file located inside bloggers nest projetc root directory.
then you need to add a [SECRET_KEY] for your project.

```
SECRET_KEY = '****************'
```
And to generate a SECRET_KEY for your project follow these steps:
open python interpreter in your terminal or commnad prompt:
and execute these commands:

```
import secrets
```
```
secrets.token_hex(16)
```
the key that is generated copy and paste it in your SECRET_KEY variable.

Now, you need to create a database file for your project. I am using SqLite database but you can use any ORM database as you like.

open python interpreter in your project root directory and execute these commands:

```
from bloggersNest import db
```
```
db.create_all()
```
after excecuting these commands you can see a site.db file is generated in you project directory.
This site.db file is added in your config.py file
```
SQLALCHEMY_DATABASE_URI = 'sqlite:///site.db'
```
lastly, add your email-id and password to these accounts, you can either add directly in to the file save it in your system environments variables and refence them here using os module, on istructions of how to do it refer youtube videoes.
```
MAIL_USERNAME = "xyz@xyz.com
```
```
MAIL_PASSWORD = "**********"
```


## Deployment

lastly open you terminal or command prompt in you project directory where run.py file i located and execute this commands:
```
pyhton run.py
```
then open the link that shows on your terminal in your browser and tada..!!

## Built With

* [Flask](http://flask.palletsprojects.com/en/1.1.x/) - The web framework used
* [python](https://www.python.org/) - programming language used


## Author

* **Abhay Singh** - *Initial work* - (https://github.com/abby2407)



