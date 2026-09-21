# Personal Task Manager

**Project Code:** WST21-PM-2026-SF  
**Student Name:** ______________________________  
**Course & Year:** ______________________________  
**Database Used:** SQLite  

## Features
- Add Task
- View Tasks
- Edit Task
- Delete Task
- Update Status (Pending / Completed)

## Technology Used
- Laravel 12
- PHP 8.2+
- Blade Views
- Eloquent Model
- SQLite Database
- Bootstrap 5 (CDN)

## Project Structure
This project demonstrates the required Laravel flow:

**Routes → Controller → Model → Database → Blade**

- `routes/web.php` — application routes
- `app/Http/Controllers/TaskController.php` — CRUD logic
- `app/Models/Task.php` — Task model
- `database/migrations/` — tasks table
- `resources/views/` — Blade pages

## How to Run

Laravel 12 requires PHP 8.2 or newer. You do not need XAMPP for this project because it uses SQLite instead of MySQL.

1. Install PHP and Composer.
2. Clone or download this repository.
3. Open a terminal inside the project folder.
4. Run:

```bash
composer install
copy .env.example .env
php artisan key:generate
php artisan migrate
php artisan serve
```

On macOS/Linux, use `cp .env.example .env` instead of `copy .env.example .env`.

5. Open the address shown by Laravel, normally `http://127.0.0.1:8000`.

## Database

The project uses SQLite. The database file is `database/database.sqlite` and the table is created by the migration when `php artisan migrate` is run.

## Notes for Submission

This repository contains the complete Laravel source project. The `vendor` folder is intentionally not included because Composer generates it from `composer.json`.
