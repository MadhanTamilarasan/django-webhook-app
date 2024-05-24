# Django Webhooks Project

Welcome to the Django Webhooks Project! This project is designed to receive data into the app server for an account and send it across different platforms (destinations) from that particular account using webhook URLs.

## Overview

The Django Webhooks Project consists of the following modules:

1. **Account Module**: Manages accounts with details such as email ID, account ID, account name, app secret token, and website (optional).
2. **Destination Module**: Manages destinations associated with accounts, including URL, HTTP method, and headers.
3. **Data Handler**: Receives JSON data via POST method, authenticates with an app secret token, identifies the account, and sends data to its destinations.

## Setup and Installation

To set up and run the Django Webhooks Project locally, follow these steps:

1. Clone the repository:
   ```bash
   git clone https://github.com/MadhanTamilarasan/django-webhook-app
   cd django-webhooks-project
2. Create a virtual environment (optional but recommended):
  ```bash
  python -m venv venv source venv/bin/activate  
3. Install dependencies:
  ```bash
  pip install -r requirements.txt
4. Apply database migrations:
  ```bash
  python manage.py migrate
5. Create a superuser:
   ```bash
   python manage.py createsuperuser
6. Run the deployment server:
  ```bash
  python manage.py runserver
7. Access the Django admin interface at http://localhost:8000/admin/ and log in with the superuser credentials.
username : madhan
password : admin@123

**API Endpoints**
The Django Webhooks Project provides the following RESTful API endpoints:

Account APIs: CRUD operations for managing accounts.
Destination APIs: CRUD operations for managing destinations.
Data Handler API: Endpoint for receiving JSON data and sending it to destinations.
