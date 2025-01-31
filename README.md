# Online Pizza Ordering App

## Overview
This is a simple web-based pizza ordering application built using Flask. The application allows users to place orders online, where API requests are sent from the client-side to the server using the `requests` module. The app also utilizes middleware to intercept requests and responses, and the `jsonify()` function is used to return JSON responses to the client.

## Features
- Users can place online pizza orders.
- API endpoints handle requests from the client side.
- The `requests` module is used for making API requests.
- Middleware is implemented to intercept and process requests and responses.
- JSON responses are sent to the client using Flask's `jsonify()`.

## Technologies Used
- **Flask** - Web framework
- **requests** - For sending API requests from the client side
- **Flask Middleware** - For intercepting requests and responses
- **Flask jsonify()** - For handling JSON responses
- **HTML, CSS, - For the frontend interface

## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/online-pizza-ordering-app.git
   cd pizza-ordering-app
   ```
2. Create a virtual environment:
   ```bash
   python -m venv my_venv
   source venv/bin/activate   # On Windows use: venv\Scripts\activate
   ```


## API Endpoints
### 1. Place an Order
- **Endpoint:** `/order`
- **Method:** `POST`
- **Request Body:**
  ```json
  {
    "customer_name": "John Doe",
    "pizza_type": "Pepperoni",
    "quantity": 2
  }
  ```
- **Response:**
  ```json
  {
    "message": "Order placed successfully",
    "order_id": 123
  }
  ```

### 2. Get Order Status
- **Endpoint:** `/order/<order_id>`
- **Method:** `GET`
- **Response:**
  ```json
  {
    "order_id": 123,
    "status": "Preparing"
  }
  ```

## Middleware
The app includes middleware that logs request and response details. It helps track API usage and monitor request flow.

## JSON Responses
The `jsonify()` function is used to send structured JSON data to the client, ensuring a consistent API response format.

## Future Enhancements
- Implement user authentication and authorization.
- Add payment gateway integration.
- Improve UI/UX with modern frontend frameworks.
- Extend order tracking functionality.



