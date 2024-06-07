## Laravel RESTful API Authentication with JWT

This project is a starter template for building a Laravel RESTful API with JWT (JSON Web Token) authentication. It provides endpoints for user registration, user login, retrieving user information, refreshing tokens, and logging out. The project is intended to serve as a boilerplate and has been uploaded to GitHub as a public repository.

## Installation

1. Clone the repository:

    ```bash
    git clone https://github.com/AlifRadifanPiandy/PHP_Laravel_StarterKit_JWT_API.git
    ```

2. Navigate to the project directory:
    ```bash
    cd PHP_Laravel_StarterKit_JWT_API
    ```
3. Install the required dependencies using Composer::

    ```bash
    composer install
    ```

4. Set up your environment variables by copying the `.env.example` file:

    ```bash
    cp .env.example .env
    ```

5. Generate a new application key:
    ```bash
    php artisan key:generate
    ```
6. Configure your database connection in the `.env` file.

7. Run the migrations:
    ```bash
    php artisan migrate
    ```
8. Generate a JWT secret key:

    ```bash
    php artisan jwt:secret
    ```

## Endpoints

| Method | Endpoint      | Description                              |
| ------ | ------------- | ---------------------------------------- |
| POST   | /api/register | Register a new user                      |
| POST   | /api/login    | User login and token generation          |
| GET    | /api/logout   | Invalidate the current token and log out |
| GET    | /api/profile  | Get current user information             |
| GET    | /api/refresh  | Refresh access token                     |

## Contributing

Pull requests are welcome. For major changes, please open an issue first
to discuss what you would like to change.

Please make sure to update tests as appropriate.

## License

This project is open-sourced software licensed under the [MIT license](https://opensource.org/licenses/MIT).
