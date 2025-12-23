# Docker Hello World App

A simple Hello World Flask application containerized with Docker, ready to deploy on Heroku.

## Features

- Simple Flask web application
- Dockerized for easy deployment
- Ready for Heroku container deployment

## Deploy to Heroku

[![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy)

## Local Development

### Run with Python

```bash
pip install -r requirements.txt
python app.py
```

### Run with Docker

```bash
docker build -t docker-hello .
docker run -p 5000:5000 -e PORT=5000 docker-hello
```

Visit `http://localhost:5000` to see the app running.

## Heroku Deployment (Manual)

1. Install the Heroku CLI
2. Login to Heroku: `heroku login`
3. Create a new app: `heroku create your-app-name`
4. Set stack to container: `heroku stack:set container`
5. Push to Heroku: `git push heroku main`

Your app will be available at `https://your-app-name.herokuapp.com`
