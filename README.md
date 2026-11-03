# RESTful GET API with Flask

## Overview

A simple RESTful API built with Python and Flask for retrieving product catalog information.

## Features

- GET request for a welcome message.
- Retrieve all products.
- Retrieve a product using its ID.
- Filter products by category.
- Return JSON responses.
- Return a 404 error when a product does not exist.
- Case-insensitive category filtering.

## API Endpoints

| Method | Endpoint | Description |
|---|---|---|
| GET | `/` | Welcome message |
| GET | `/products` | Retrieve all products |
| GET | `/products/2` | Retrieve product with ID 2 |
| GET | `/products?category=books` | Filter products by category |

## Example Responses

### Homepage

`GET /`

Returns a welcome message in JSON.

### All Products

`GET /products`

Returns a list of available products.

### Single Product

`GET /products/2`

Returns the Book product.

### Category Filter

`GET /products?category=books`

Returns products belonging to the books category.

### Missing Product

`GET /products/99`

Returns a JSON error with HTTP status 404.

## Installation

Install dependencies:

`pipenv install`

## Run the Application

`pipenv run python app.py`

The API runs at `http://127.0.0.1:5000`.

## Run Tests

`pipenv run python -m pytest -v`

## Technologies

- Python
- Flask
- JSON
- Pytest

## Author

Abdulsalam
