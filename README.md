# Chirper 🐦

Chirper is a modern microblogging platform built with Laravel 12. It allows users to share short messages, view a global feed, and manage their own posts in real-time.

This project was built during the Laravel Bootcamp to master the fundamentals of the PHP ecosystem, modern routing, and secure database interactions.


---

## ✨ Features

- **Secure Authentication:** Custom-built login, registration, and logout flows using specialized Invokable Controllers.
- **Optimized Feed:** Displays the latest 50 chirps with Eager Loading to ensure high performance.
- **Full CRUD:** Complete ability to Create, Read, Update, and Delete chirps.
- **Data Protection:** Uses Laravel's authorization logic to ensure users can only manage their own content.
- **Modern UI:** Responsive interface powered by Tailwind CSS and DaisyUI.

## 🛠️ Tech Stack

- **Framework:** Laravel 12
- **Language:** PHP 8.2+
- **Database:** MySQL
- **Frontend:** Blade Components, Tailwind CSS, DaisyUI

---

## 🚀 Installation & Setup

Follow these steps to get your local environment running:

### 1. Clone & Install
- git clone https://github.com/MLama2059/chirper.git
- cd chirper
- composer install
- npm install && npm run build

### 2. Environment Setup
- Copy the template file: `cp .env.example .env`
- Open the `.env` file and verify your **MySQL** settings:
  DB_CONNECTION=mysql, 
  DB_HOST=127.0.0.1, 
  DB_PORT=3306, 
  DB_DATABASE=chirper, 
  DB_USERNAME=root, 
  DB_PASSWORD=
- Generate the application key: `php artisan key:generate`

### 3. Database & Launch
- Run: php artisan migrate
- Run: php artisan serve

---

## 📂 Project Structure

- App/Http/Controllers/Auth/: Specialized auth logic using single-action classes.
- App/Models/Chirp.php: Character limits and user-ownership logic.
- resources/views/: Modular UI components using a central <x-layout> component.

## 📜 License

This project is open-sourced software licensed under the [MIT license](https://opensource.org/licenses/MIT).
