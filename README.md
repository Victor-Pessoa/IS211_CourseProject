# IS211_CourseProject
Solution
This is a blog application built with Flask, a micro web framework written in Python. It utilizes the Flask-SQLAlchemy extension for database management, Flask-Bcrypt for password hashing and Flask-Login for user session management.

Upon loading the application, a user is presented with a list of available blog posts ordered in reverse chronological order. Users can log in via the '/login' URL and upon successful login, they're directed to the '/dashboard' page.

Here, users can view all their blog posts, edit or delete them, and create new ones. Each blog post has a unique URL, called a permalink, which can be accessed directly. There's also a feature for users to 'unpublish' their posts, making them unavailable for viewing on the website.

The application also supports categorization of blog posts. Users can create categories and associate their blog posts with these categories. Each category has a dedicated page that displays all the blog posts under it.

Model Structure
The models used in this application are defined in the models.py file. Here are the primary models:

User: This model represents the users of the application. Each user has a username, password, and email. The User model has a one-to-many relationship with the Post model, meaning a user can have many posts.

Post: This model represents the blog posts. Each post has a title, content, published date, author (user), and category. The Post model has a many-to-one relationship with the Category model.

Category: This model represents the post categories. Each category has a name, and can be associated with many posts.

Files and Modules
Here is a breakdown of the different files and modules used in this application:

run.py: This is the main entry point of the application. It creates an instance of the application and runs it.

__init__.py: This file initializes the Flask application and the database, and imports the routes.

routes.py: This file defines all the routes for the application. It also includes view functions that handle the logic for each route.

config.py: This file contains the configuration variables for the application.

forms.py: This file contains the Flask-WTF form classes for the login, registration, and blog post forms.

models.py: This file defines the SQLAlchemy models used in the application.

templates/: This directory contains all the Jinja2 templates used for the UI of the application.

static/: This directory contains static files like CSS and JavaScript.

Running the Application
Ensure that you have Python 3.6 or later installed on your machine. Also, install the necessary dependencies by running pip install -r requirements.txt in the root directory of the project.

To start the application, navigate to the root directory in the command line and run the command python run.py. The application will start running on http://localhost:5000.
