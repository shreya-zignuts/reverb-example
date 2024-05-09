<p align="center">
    <img src="https://reverb.laravel.com/socialcard.png" width="50%" alt="laravel reverb logo">
</p>
<p align="center">
    <img src="https://logowik.com/content/uploads/images/laravel-livewire4180.logowik.com.webp" width="50%" alt="laravel livewire logo">
</p>


## Introduction

Laravel Reverb is a first-party WebSocket server for Laravel applications, providing real-time communication capabilities between the client and server seamlessly.

Laravel Reverb has numerous appealing features, including:

- Speed and scalability.
- Support for thousands of simultaneous connections.
- Integration with existing Laravel broadcasting features.
- Compatibility with Laravel Echo.
- First-class integration and deployment with Laravel Forge.

- I love to start new Laravel apps with one of the starter kits that ships with login, registration, email verification, etc. In this, I’ll use Laravel JetStream with Livewire.

## Official Documentation

Documentation for Reverb can be found on the [Laravel website](https://laravel.com/docs/reverb).

## Contributing

Thank you for considering contributing to Reverb! The contribution guide can be found in the [Laravel documentation](https://laravel.com/docs/contributions).

## Code of Conduct

In order to ensure that the Laravel community is welcoming to all, please review and abide by the [Code of Conduct](https://laravel.com/docs/contributions#code-of-conduct).

## Security Vulnerabilities

Please review [our security policy](https://github.com/laravel/reverb/security/policy) on how to report security vulnerabilities.

## License

Laravel Reverb is open-sourced software licensed under the [MIT license](LICENSE.md).

## Requirements

- PHP >= 8.1
- Composer
- Node.js >= 21.6.2
- NPM >= 10.2.4
- MySQL

## installation

Step 1: Clone the Repository

Clone the repository to your local machine using Git (branch - develop)

```bash
$ git clone https://github.com/shreya-zignuts/reverb-example.git
```

Step 2: Navigate to the Project Directory

Change your current directory to the project directory.

```bash
$ cd reverb-example
```

Step 3: Follow the steps as for creating laravel app

- composer install
- npm install

Step 4: Install Laravel Reverb

We need to install Laravel Reverb – our WebSocket Server into the Laravel app.

```bash
$ php artisan install:broadcasting
```

Step 5: New Terminal Start Reverb Server

```bash
$ php artisan reverb:start
```

Step 6: New Terminal Run Vite 

```bash
$ npm run dev
```

Step 7: New Terminal, ensure your queue running

```bash
$ php artisan queue:listen
```

Step 8: Generate Application Key

Generate an application key.

```bash
$ php artisan key:generate
```

Step 9: Configure Database Connection

Configure your database connection in the .env file.

```make
DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=your_database_name
DB_USERNAME=your_database_username
DB_PASSWORD=your_database_password
```

Step 10: Run Migrations and Seeders

Run database migrations and seeders to create database tables and populate them with initial data.

```bash
$ php artisan migrate --seed
```

Step 11: Start the Development Server

Start the development server to run the application.

```bash
$ php artisan serve
```

Step 12: Access the Application

Open your web browser and visit http://localhost:8000 to access the application.
