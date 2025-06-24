# Flask-Docker-App
A simple Flask web application using Docker.

Here's a step-by-step guide:

# Create a Dockerfile:

Use the official Python image python:3.8-slim as the base.

Command: FROM python:3.8-slim

Run the command pip install Flask to install Flask.

Command: RUN pip install Flask

Copy your application code app.py into the Docker image at the path /app/.

Command: COPY app.py /app/

Set the default command to start the Flask app using the Python interpreter. To do this, instruct it to execute python /app/app.py.

Command: CMD ["python", "/app/app.py"]

# Build the Docker Image:
Using "docker build -t flask-docker-app python-project", if we want to execute in the current directory, we can use this 

or else

Using "docker build -t flask-docker-app", we can create a Docker image in the Docker file directory

Use the command line to build the image from your Dockerfile.
