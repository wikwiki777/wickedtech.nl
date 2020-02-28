# wickedtech.nl

Personal Blog, Portofolio, Resume

Website to:

- Post blog items
- Showcase portofolio
- Showcase Resume/Certifications

Table of contents :

- [Technologies Used](#Technologies-Used)
- [Features](#Features)
- [UI/UX](#UI/UX)
- [Database](#Database)
- [Testing](#Testing)
- [Deployment](#Deployment)
  - [Local setup](#Local-setup)
  - [Production deployment](#Production-deployment)

## Technologies Used

- Python3
- Django3
- Postgresql10+
- python-dotenv
- dj-database-url

[***TOP***](#wickedtech.nl)

## Features

[***TOP***](#wickedtech.nl)

## UI/UX

[***TOP***](#wickedtech.nl)

## Database

[***TOP***](#wickedtech.nl)

## Testing

[***TOP***](#wickedtech.nl)

## Deployment

### Local setup

1. Create a virtualenv and activate it

    ```bash
    # Create a virtualenv
    # Change envname to your desired name.
    $virtualenv envname

    $python3 -m venv envname

    # Go into your newly created virtualenv
    $cd envname

    # Activate the virtualenv
    $source bin/activate
    ```

2. Clone/Download this repo and place the files in your newly created virtalenv

    ```dirtree
    # Example folder tree
    envname/
        |bin/
        |djangoProject/
        |include/
        |lib/
        |lib64/
        |share/
        |.env
        |.gitignore
        |db.sqlite3
        |pyvenv.cfg
        |README.md
    ```

3. Install the python packages in requirements.txt

    ```bash
    $pip install -r requirements.txt
    ```

4. Create a .env file in the root directory of your virtualenv
with the following contents.

    ```envfile
    #https://pypi.org/project/python-dotenv/

    #SET DEBUG: 1 is True, empty is False
    DEVELOPMENT = 1

    #Secret key required by django
    #i.e. generate one here  https://djskgen.herokuapp.com/
    SECRET_KEY = ""

    #Database urls https://pypi.org/project/dj-database-url/
    #https://github.com/jacobian/dj-database-url
    DEV_DATABASE_URL = "sqlite:///db.sqlite3"
    PROD_DATABASE_URL = ""

    #Set Email: 1 is Console, empty is SMTP
    EMAIL = 1
    EMAIL_ADDRESS = ""
    EMAIL_PASSWORD = ""
    ```

[***TOP***](#wickedtech.nl)

### Production deployment

We will be deploying to a vps running ubuntu server 18.04 LTS with
Plesk Obsidian 18 installed.

***Todo:***

***Plesk instructions for hosting a python application here***

[***TOP***](#wickedtech.nl)

## Credits

[***TOP***](#wickedtech.nl)

### Media
