# E-commerce Backend

Welcome to the E-commerce Backend repository. This backend system is built using **Spring Boot** and is designed to handle various operations essential for an online store, including user management, product handling, order processing, and more.

## Features

- **User Management:** Handles user registration, authentication, and profile management.
- **Product Management:** Allows for adding, updating, deleting, and retrieving product information.
- **Order Processing:** Manages customer orders, including creation, updating, and retrieval.
- **Shopping Cart:** Facilitates adding, removing, and updating products in a user's shopping cart.
- **Payment Integration:** Integrates with payment gateways for processing transactions securely.
- **Security:** Implements authentication and authorization mechanisms to protect user data and system integrity.

## Installation

1. **Clone the Repository:**

   ```bash
   git clone https://github.com/RaviSKumar210755/Ecommerce-Backend.git
   ```

2. **Navigate to the Project Directory:**

   ```bash
   cd Ecommerce-Backend
   ```

3. **Install Dependencies:**

   ```bash
   mvn install
   ```

4. **Set Up Environment Variables:**

   - Create an `application.properties` file in the `src/main/resources` directory.
   - Define necessary environment variables such as `server.port`, `spring.datasource.url`, `spring.datasource.username`, `spring.datasource.password`, etc.

5. **Run the Application:**

   ```bash
   mvn spring-boot:run
   ```

   The server should now be running on the specified port.

## API Endpoints

### User Endpoints

- **Register a New User**
  - `POST /api/users/register`
  - Registers a new user.
  - **Request Body:**
    ```json
    {
      "username": "string",
      "email": "string",
      "password": "string"
    }
    ```

- **User Login**
  - `POST /api/users/login`
  - Authenticates a user and returns a token.

- **Get User Profile**
  - `GET /api/users/profile`
  - Retrieves the profile of the authenticated user.

### Product Endpoints

- **Get All Products**
  - `GET /api/products`
  - Retrieves a list of all products.

- **Get Product by ID**
  - `GET /api/products/{id}`
  - Retrieves details of a specific product.

- **Create a New Product (Admin only)**
  - `POST /api/products`
  - Creates a new product.

- **Update a Product (Admin only)**
  - `PUT /api/products/{id}`
  - Updates an existing product.

- **Delete a Product (Admin only)**
  - `DELETE /api/products/{id}`
  - Deletes a product.

### Order Endpoints

- **Create a New Order**
  - `POST /api/orders`
  - Creates a new order.

- **Get User Orders**
  - `GET /api/orders`
  - Retrieves all orders of the authenticated user.

- **Get Order by ID**
  - `GET /api/orders/{id}`
  - Retrieves details of a specific order.

## Contributing

Contributions are welcome! Please fork the repository and submit a pull request for any enhancements or bug fixes.

## License

This project is licensed under the MIT License. See the `LICENSE` file for details.

