# Book Registration and Viewing

A Laravel 12 lab project using PHP, MySQL, Blade, and Bootstrap. Users can register/login and manage a personal reading list. Each account sees only its own books.

## Requirements

- PHP 8.2 or later with the PHP extensions required by Laravel
- Composer
- MySQL or MariaDB (for example, via XAMPP)
- Git (for GitHub upload)

## Install

1. Create a MySQL database named `book_registration`.
2. Copy `.env.example` to `.env`.
3. Set your local database username/password in `.env`.
4. From the project directory, run:

   ```bash
   composer install
   php artisan key:generate
   php artisan migrate
   php artisan serve
   ```

5. Visit `http://127.0.0.1:8000/register`.

If `php` is not on PATH in Windows with XAMPP, use `C:\\xampp\\php\\php.exe artisan ...`.

## Bootstrap and offline use

The views load Bootstrap from a CDN, so styling needs internet access. The application itself runs locally once Composer dependencies are installed and the database server is running.

## GitHub

Do not commit `.env`, `vendor/`, or `node_modules/`. Commit `.env.example` and source code instead. Never upload passwords or real user data.

## Notes

This archive contains the application source and Laravel project configuration, not the generated `vendor/` dependencies. Run `composer install` to create `vendor/` on the target computer.
