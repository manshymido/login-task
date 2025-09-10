# Authentication System

A modern authentication system built with Laravel that provides user registration, login, and profile management functionality.

## Features

- User Registration
- User Login/Logout
- Password Reset
- Email Verification
- User Profile Management
- Remember Me Functionality
- Secure Password Handling
- Protected Dashboard

## Requirements

- PHP >= 8.1
- Composer
- Node.js & NPM
- MySQL
- XAMPP/WAMP/MAMP or similar local development environment

## Installation

1. Clone the repository
```bash
git clone https://github.com/manshymido/login-task.git
```

2. Navigate to the project directory
```bash
cd login-task
```

3. Install PHP dependencies
```bash
composer install
```

4. Install NPM dependencies
```bash
npm install
```

5. Create and configure environment file
```bash
cp .env.example .env
```

6. Generate application key
```bash
php artisan key:generate
```

7. Configure your database in `.env` file
```env
DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=login
DB_USERNAME=root
DB_PASSWORD=
```

8. Run database migrations
```bash
php artisan migrate
```

9. Build assets
```bash
npm run dev
```

10. Start the local development server
```bash
php artisan serve
```

The application will be available at `http://localhost:8000`

## Usage

### Registration
- Visit `/register` to create a new account
- Fill in your name, email, and password
- Submit the form to create your account

### Login
- Visit `/login` to access your account
- Enter your email and password
- Use the "Remember me" option to stay logged in

### Dashboard
- After logging in, you'll be redirected to the dashboard
- View your profile information
- Access various protected features

### Profile Management
- Click on your name in the navigation
- Select "Profile" to edit your information
- Update your name, email, or password
- Delete your account if needed

## Security

- All passwords are hashed
- Protection against CSRF attacks
- Session-based authentication
- Secure password reset process
- Protected routes using middleware

## License

This project is open-sourced software licensed under the [MIT license](https://opensource.org/licenses/MIT).
