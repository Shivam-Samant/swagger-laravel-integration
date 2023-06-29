# Laravel Swagger Integration

This project demonstrates the integration of Swagger documentation into a Laravel application. It provides an example implementation of login and register routes, along with Swagger documentation for these routes.

## Installation

Follow these steps to set up the project on your local machine:

1. Clone the repository:

    ```sh 
    git clone https://github.com/Shivam-Samant/swagger-laravel-integration.git
    ```

1. Navigate to the project directory:

    ```sh
    cd laravel-swagger-integration
    ```

1. Install the dependencies using Composer:

    ```sh
    composer install
    ```

1. Copy the .env.example file and rename it to .env:

    ```sh
    cp .env.example .env
    ```

1. Generate an application key:

    ```sh
    php artisan key:generate
    ```

1. Set up your database configuration in the .env file.

1. Migrate the database:

    ```sh
    php artisan migrate
    ```

1. Publish the L5Swagger assets and configuration files:

    ```sh
    php artisan vendor:publish --provider "L5Swagger\L5SwaggerServiceProvider"
    ```

1. Generate the Swagger JSON documentation:

    ```sh
    php artisan l5-swagger:generate
    ```
    This command will generate a Swagger JSON file based on the annotations in your route files and controller methods.

1. Serve the application:

    ```sh
    php artisan serve
    ```
    The application will be accessible at `http://localhost:8000`

## Swagger Documentation

The Swagger documentation is automatically generated based on the annotations in your route files and controller methods. To view the Swagger documentation, follow these steps:

1. Start the Laravel development server:

    ```sh
    php artisan serve
    ```
2. Open your browser and navigate to `http://localhost:8000/api/documentation`.

    This will display the Swagger UI, where you can explore the available endpoints, make requests, and view the API documentation.