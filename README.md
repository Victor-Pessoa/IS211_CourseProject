# IS211_CourseProject
Introduction
Welcome to My Flask Blog! This is a simple yet functional web application built with Flask, a micro web framework written in Python. Users can register, log in, and create their own blog posts.

Requirements
This application is built with the following technologies:

Python 
Flask
Jinja2 (for templates)

Installation
To set up this application, follow these steps:

Clone the repository.
Install Python if you haven't already.
Create a virtual environment: python -m venv env
Activate the virtual environment:
On Windows: env\Scripts\activate
On Unix or MacOS: source env/bin/activate
Install the necessary dependencies (listed in the requirements.txt file): pip install -r (Flask,Flask-SQLAlchemy,Flask-WTF,Flask-Login,flask-migrate)
Start the Flask server: run the run.py file

Usage
Once you've started the server, you can navigate to localhost:5000 (or wherever your Flask server is running) in your web browser.

Register: Click the Register link to create an account.
Login: Click the Login link to log in to your account.
Creating a post: Once logged in, you can create blog posts from your dashboard.

File Structure
Here is an overview of the main files and directories in this project:

dashboard.html: The user's dashboard, where they can create new posts.
index.html: The home page, which displays all blog posts.
login.html: The login page.
post.html: The page for viewing a single post.
register.html: The registration page, where new users can create an account.

* To start the application, navigate to the root directory in the command line and run the command python run.py. The application will start running on http://localhost:5000.
