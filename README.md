# Django Task Management System API

## Overview

This project is a RESTful API for a Task Management System built with Django and Django REST Framework (DRF). It allows users to perform CRUD operations on tasks with properties such as title, description, status, priority, and due date. The project includes advanced features like custom filters and efficient logging.

## Features

- **Task Management:** Create, read, update, and delete tasks.
- **Filtering:** Filter tasks based on status, priority, and due date.
- **Logging:** Detailed logging setup for development and production environments.
- **HIGHLY CUSTOMIZABLE:**  highly costomizable class based views, serializers, 
- **Advance Modular and Reusable Code:** by use of Mixins, Method Overriding, Custom TestCases, and many more
- **Caching:** i have used caching for reduce database load in production we can use distributed cache like redis or memcach with connection pooling
- **Faker:**  Generate fake data for testing purpose. using "python create_fake_data.py" or "python manage.py create_fake_data" 
- **Pagination:** for large response data, i implemeneted pagination for quick response
- **Documentation:** API documentation using DRF-YASG.


### Prerequisites

- Python 3.8+

### Setup

1. **Clone the Repository:**

   ```bash
   git clone <repository-url>
   cd <repository-directory>
Install Dependencies:

Create a virtual environment (recommended) and install the required packages:

python -m venv venv
source venv/bin/activate  # On Windows use `venv\Scripts\activate`
pip install -r requirements.txt
Configure Environment:

Ensure your .env file or environment variables are set up for database and secret key settings.

Run Migrations:
python manage.py  makemigrations
python manage.py migrate

Create a Superuser:
python manage.py createsuperuser

Run the Development Server:
Start the development server to run the API:

python manage.py runserver

optional:
  in other ternimal use can use this to Generate fake data for testing purpose. 
    "python create_fake_data.py" or "python manage.py create_fake_data" 

API Endpoints
GET api/tasks/: Retrieve a list of tasks.
GET api/tasks/<id>/: Retrieve details of a specific task by its ID.
POST api/tasks/: Create a new task.
PUT api/tasks/<id>/: Update an existing task.
DELETE api/tasks/<id>/: Delete a specific task.


Example Request
Create Task:
POST /tasks/
Content-Type: application/json

{
  "title": "Fix bug",
  "description": "Fix the bug in module X",
  "status": "To Do",
  "priority": "High",
  "due_date": "2024-08-15"
}
Logging
The project uses Django’s logging framework with both file and console handlers. Logs are stored in the logs/django.log file.

API Documentation
API documentation is available at /swagger/ (configured using DRF-YASG).

Testing
Ensure you have all dependencies installed and run tests with:

python manage.py test
or 
pytest


For any questions or comments, please contact shuaibansari4044@gmail.com.

### Key Points

- **Setup Instructions:** Step-by-step guide to getting the project up and running.
- **API Endpoints:** Basic information on available endpoints.
- **Logging Configuration:** Basic information on logging.
- **Documentation URL:** Where to find the auto-generated API documentation.
- **Contributing:** Instructions for contributing to the project.





