# Simple API with Basic Authentication

This project is a simple REST API built with Flask. It includes basic authentication and a single model, `User`. The API provides endpoints to interact with user data and check the status of the server.

## Table of Contents

- [Project Overview](#project-overview)
- [Setup and Installation](#setup-and-installation)
- [Running the Application](#running-the-application)
- [API Endpoints](#api-endpoints)
- [Testing](#testing)
- [Development and Deployment](#development-and-deployment)
- [Troubleshooting](#troubleshooting)
- [License](#license)

## Project Overview

This project contains a simple API with the following features:
- Basic authentication using Base64 encoding.
- A `User` model with file-based storage.
- Endpoints to check the status of the server and interact with user data.

## Setup and Installation

Follow these steps to set up the project:

1. **Clone the Repository:**

   ```bash
   git clone https://github.com/yourusername/alx-backend-user-data.git
# Simple API with Basic Authentication

This project is a simple REST API built with Flask. It includes basic authentication and a single model, `User`. The API provides endpoints to interact with user data and check the status of the server.

## Table of Contents

- [Project Overview](#project-overview)
- [Setup and Installation](#setup-and-installation)
- [Running the Application](#running-the-application)
- [API Endpoints](#api-endpoints)
- [Testing](#testing)
- [Development and Deployment](#development-and-deployment)
- [Troubleshooting](#troubleshooting)
- [License](#license)

## Project Overview

This project contains a simple API with the following features:
- Basic authentication using Base64 encoding.
- A `User` model with file-based storage.
- Endpoints to check the status of the server and interact with user data.

## Setup and Installation

Follow these steps to set up the project:

1. **Clone the Repository:**

   ```bash
   git clone https://github.com/yourusername/alx-backend-user-data.git
# Simple API with Basic Authentication

This project is a simple REST API built with Flask. It includes basic authentication and a single model, `User`. The API provides endpoints to interact with user data and check the status of the server.

## Table of Contents

- [Project Overview](#project-overview)
- [Setup and Installation](#setup-and-installation)
- [Running the Application](#running-the-application)
- [API Endpoints](#api-endpoints)
- [Testing](#testing)
- [Development and Deployment](#development-and-deployment)
- [Troubleshooting](#troubleshooting)
- [License](#license)

## Project Overview

This project contains a simple API with the following features:
- Basic authentication using Base64 encoding.
- A `User` model with file-based storage.
- Endpoints to check the status of the server and interact with user data.

## Setup and Installation

Follow these steps to set up the project:

1. **Clone the Repository:**

   ```bash
   git clone https://github.com/yourusername/alx-backend-user-data.git

2.Navigate to the Project Directory:

cd alx-backend-user-data/0x01-Basic_authentication/SimpleAPI

3.Install Dependencies:

Ensure you have Python 3.7 installed. Then, install the required Python packages:

pip3 install -r requirements.txt

4. Resolve Dependencies (if needed):

pip3 install --upgrade --force-reinstall -r requirements.txt

Running the Application

To start the Flask application, use the following command:

API_HOST=0.0.0.0 API_PORT=5000 python3 -m api.v1.app

The application will be available at the following addresses:

http://127.0.0.1:5000
http://<YOUR_IP>:5000 (Replace <YOUR_IP> with your local IP address if needed)

API Endpoints
/api/v1/status
Method: GET

Description: Returns the status of the API.

Response:

{
  "status": "OK"
}


Testing
To test the API, you can use curl or any HTTP client. For example:

curl http://127.0.0.1:5000/api/v1/status

Development and Deployment
For development purposes, the built-in Flask server is sufficient. However, for production deployments, consider using a WSGI server like Gunicorn.

Install Gunicorn:

pip3 install gunicorn

Run with Gunicorn:

gunicorn -b 0.0.0.0:5000 api.v1.app:app


Troubleshooting
Dependency Issues: If you encounter issues with package versions, make sure to resolve conflicts and install compatible versions as specified in requirements.txt.
Server Not Starting: Ensure all dependencies are correctly installed and there are no syntax errors in the code.

LICENSE 

This project is linsed under the MIT License.See the LICENCE file for details.

Feel free to contribute to this project or raise issues if you encounter any problems.

For more information, contact inganathi2001@gmail.com.

Give me a Star to show your appreciation :)
