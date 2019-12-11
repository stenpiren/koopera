Koopera
=========

Koopera is a code review app for adding comments directly on `.ipynb` files

# Features
* Add comments directly in notebooks cells for .ipynb files
* Github authentication via personal access token

![demo](docs/demo.gif)

# Quickstart
You can easily start using Koopera with docker. You can get the image from [docker hub](https://hub.docker.com/r/rsn491/koopera) or build it from the source.

If you want to build, please run the cmd below:

`docker build -t koopera .`

To start the app, please run the cmd below:

`docker run -p 8080:8080 koopera`
    
The app can now be accessed at: [http://0.0.0.0:8080](http://0.0.0.0:8080)


# Setting up dev environment

## Dependencies
* Python 3.6
* nodejs 10

## Setting up backend for local development

1. Enable CORS by setting `ALLOW_CORS` to `True` in [src/backend/config.py](src/backend/config.py)

2. Create virtualenv

    `python -m venv venv`
    
3. Activate virtualenv

    `source venv/bin/activate`

4. Install dependencies
    
    `pip install -r requirements.txt`

5. Start flask app on default port (5000)

    `python run.py`

## Setting up frontend for local development

1. Install dependencies

    `npm install`
2. Run web server for serving frontend

    `npm run serve`
    
A web server for serving frontend with hot reload will be listening on 
[http://localhost:8080](http://localhost:8080)


# Credits 

<div>Icons made by <a href="https://www.flaticon.com/authors/nikita-golubev" title="Nikita Golubev">Nikita Golubev</a> from <a href="https://www.flaticon.com/"                 title="Flaticon">www.flaticon.com</a> is licensed by <a href="http://creativecommons.org/licenses/by/3.0/"                 title="Creative Commons BY 3.0" target="_blank">CC 3.0 BY</a></div>
