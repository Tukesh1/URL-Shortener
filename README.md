# URL Shortener

Welcome to the URL Shortener! This project is a simple web application built using PHP that allows users to shorten long URLs into more manageable and easy-to-share short URLs.

## Features

- Shorten long URLs
- Redirect from short URLs to the original long URLs
- Simple and user-friendly interface

## Requirements

- PHP 7.0 or higher
- MySQL or any other compatible database

## Installation

1. **Clone the Repository:**

   ```bash
   git clone https://github.com/Tukesh1/URL-Shortener.git
   cd url-shortener
   ```

2. **Database Setup:**

   - Create a new database in your MySQL server.
   - Import the provided SQL file to set up the necessary tables. Run the following command in your MySQL client:

     ```sql
     CREATE DATABASE url_shortener;
     USE url_shortener;
     SOURCE path/to/your/url_shortener.sql;
     ```

3. **Configuration:**

   - Rename the `config.example.php` file to `config.php`.
   - Open `config.php` and update the database configuration details:

     ```php
     <?php
     // Database configuration
     $db_host = 'localhost'; // Database host
     $db_user = 'root'; // Database username
     $db_pass = 'password'; // Database password
     $db_name = 'url_shortener'; // Database name
     ?>
     ```

4. **Start the Server:**

   - Place the project files in your web server's root directory (e.g., `htdocs` for XAMPP or `www` for WAMP).
   - Start your web server (e.g., Apache) and ensure PHP is running.

## Usage

1. **Access the Application:**

   Open your web browser and navigate to `http://localhost/url-shortener`.

2. **Shorten a URL:**

   - Enter the long URL you want to shorten in the input field.
   - Click the "Shorten" button.
   - The shortened URL will be displayed, and you can copy it for sharing.

3. **Redirect to Long URL:**

   - Use the shortened URL in your browser's address bar.
   - The application will automatically redirect you to the original long URL.

## Project Structure

- `index.php`: The main file containing the URL shortener form and logic.
- `redirect.php`: Handles redirection from short URLs to long URLs.
- `config.php`: Configuration file for database connection.
- `db.sql`: SQL file for creating the necessary database tables.

---

Thank you for using the URL Shortener! We hope you find it useful.
