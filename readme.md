# Developing RESTful APIs with Python, Django, and Django Rest Framework

This repository contains the code for developing RESTful APIs using Python, Django, and Django Rest Framework. 

## Prerequisites

Before getting started, make sure you have the following installed:

- Python 
- Django
- Django Rest Framework 

## Installation

1. Clone the repository:

    ```shell
    git clone https://github.com/yarragotiravitheja/djangoapi.git
    ```

2. Create a virtual environment:

    ```shell
    python -m venv venv
    ```

3. Activate the virtual environment:

    - For Windows:

      ```shell
      venv\Scripts\activate
      ```

    - For macOS/Linux:

      ```shell
      source venv/bin/activate
      ```

4. Install the required dependencies:

    ```shell
    pip install -r requirements.txt
    ```

## Usage

1. Run the development server:

    ```shell
    python manage.py runserver
    ```

2. Open your web browser and navigate to `http://localhost:8000/api/` to access the API endpoints.



Now you can send requests to your API via Postman, your app or do a GETrequests from your browser, examples:

```
POST /api/v1/posts/create/
HTTP 200 OK
Allow: POST, OPTIONS
Content-Type: application/json
Vary: Accept

{
    "status_code": 200,
    "message": "Successfully created",
    "result": {
        "csrfmiddlewaretoken": "rnSUN3XOIghnXA0yKghnQgxg0do39xhorYene5ALw3gWGThK5MjG6YjL8VUb7v2h",
        "title": "Creating a resource",
        "content": "Howdy mate!"
    }
}
GET /api/v1/posts/1/
HTTP 200 OK
Allow: GET, PUT, PATCH, DELETE, HEAD, OPTIONS
Content-Type: application/json
Vary: Accept

{
    "status_code": 200,
    "message": "Successfully retrieved",
    "result": {
        "title": "Sample Post",
        "content": "Sample Post Content",
        "is_featured": false
    }
}
```

That’s it. You have successfully managed to develop RESTful APIs with DRF! Cheers!

## Contributing

Contributions are welcome! If you find any issues or have suggestions for improvement, please open an issue or submit a pull request.

