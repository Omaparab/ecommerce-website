# Ecommerce Website

A Django-based e-commerce web application for selling stationery and office supplies. The project includes product browsing, user signup/login, checkout, and order confirmation workflows, making it a simple full-stack storefront example built with Python and Django.

## Overview

This application simulates a modern online shopping experience for office and school essentials. Customers can browse product pages, create an account, log in, place an order, and receive an order ID after completing the purchase flow.

## Features

- User registration and login flow
- Product pages for stationery and office items
- Cart and checkout pages
- Order placement form with customer details
- Random order ID generation for successful purchase confirmation
- SQLite database for storing users and purchase records
- Static assets and templates for a storefront UI

## Tech Stack

- Python
- Django 5.1
- SQLite
- HTML/CSS templates
- Gunicorn (included for deployment)

## Project Structure

```text
 ecommerce-website/
 ├── README.md
 └── myProject/
     ├── myApp/
     │   ├── static/
     │   ├── templates/
     │   ├── models.py
     │   ├── views.py
     │   └── ...
     ├── myProject/
     │   ├── settings.py
     │   ├── urls.py
     │   └── wsgi.py
     ├── db.sqlite3
     ├── manage.py
     ├── requirements.txt
     ├── render.yaml
     └── runtime.txt
```

## Main Functionalities

- `home`: landing page
- `login`: user authentication
- `signup`: create a new customer account
- `cart`: shopping cart page
- `checkout`: order review page
- `buy`: capture customer data before purchase
- `proceed`: generate and display a confirmation order ID
- Product pages: `calci`, `drafter`, `folder`, `geometry`, `punch`, `raspberry`, `sheetholder`, `stapler`

## Setup Instructions

1. Open a terminal and go to the project folder:

```bash
cd ecommerce-website/myProject
```

2. Create and activate a virtual environment:

```bash
python -m venv myenv
myenv\Scripts\activate
```

3. Install dependencies:

```bash
pip install -r requirements.txt
```

4. Apply database migrations:

```bash
python manage.py migrate
```

5. Start the development server:

```bash
python manage.py runserver
```

6. Visit the app in your browser:

```text
http://127.0.0.1:8000/
```

## Creating an Admin User

```bash
python manage.py createsuperuser
```

Then log in to the Django admin panel at:

```text
http://127.0.0.1:8000/admin/
```

## Deployment

The project includes a `render.yaml` configuration for deployment on Render using Gunicorn.

## Notes

This is a learning/demo storefront and can be extended with features such as:

- product categories and search
- cart persistence
- payment integration
- admin product management
- order history and user profiles

