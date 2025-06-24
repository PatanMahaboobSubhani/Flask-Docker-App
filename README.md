# Flask-Docker-App
A simple Flask web application using Docker.

Here's a step-by-step guide:

Create a Dockerfile:

Use the official Python image python:3.8-slim as the base.

Run the command pip install Flask to install Flask.

Copy your application code app.py into the Docker image at the path /app/.

Set the default command to start the Flask app using the Python interpreter. You can achieve this by instructing it to execute python /app/app.py.

Build the Docker Image:

Use the command line to build the image from your Dockerfile.
