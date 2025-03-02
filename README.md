# Restaurant Delivery API

This project is a simple Restaurant Delivery API built with FastAPI. It allows users to interact with restaurants, manage orders, and handle user authentication. The API is designed to be lightweight and user-friendly, making it easy to extend and modify.

## Features

- User authentication (login and registration)
- Manage restaurants (add, list)
- Manage orders (create, retrieve)
- User profile management

## Project Structure

```
restaurant-delivery-api
├── src
│   ├── app.py                # Entry point of the application
│   ├── controllers           # Contains business logic for handling requests
│   │   ├── auth.py           # User authentication functions
│   │   ├── orders.py         # Order management functions
│   │   ├── restaurants.py     # Restaurant management functions
│   │   └── users.py          # User management functions
│   ├── models                # Database models
│   │   ├── order.py          # Order model
│   │   ├── restaurant.py      # Restaurant model
│   │   └── user.py           # User model
│   ├── schemas               # Pydantic schemas for validation
│   │   ├── order.py          # Order schema
│   │   ├── restaurant.py      # Restaurant schema
│   │   └── user.py           # User schema
│   ├── db                   # Database connection logic
│   │   └── database.py       # Database setup
│   └── routers               # API route definitions
│       ├── auth.py           # Authentication routes
│       ├── orders.py         # Order routes
│       ├── restaurants.py      # Restaurant routes
│       └── users.py          # User routes
├── tests                     # Unit tests for the API
│   └── test_api.py          # Test cases for API endpoints
├── requirements.txt          # Project dependencies
├── .env                      # Environment variables
└── README.md                 # Project documentation
```

## Installation

1. Clone the repository:
   ```
   git clone <repository-url>
   ```

2. Navigate to the project directory:
   ```
   cd restaurant-delivery-api
   ```

3. Install the required dependencies:
   ```
   pip install -r requirements.txt
   ```

4. Set up your environment variables in the `.env` file.

## Usage

To run the application, execute the following command:
```
uvicorn src.app:app --reload
```

Visit `http://localhost:8000` to access the API documentation and test the endpoints.

## Contributing

Contributions are welcome! Please open an issue or submit a pull request for any improvements or features you'd like to add.

## License

This project is licensed under the MIT License.