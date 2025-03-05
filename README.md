# Connectify App


## Overview
**Connectify App** is a real-time chat application designed for seamless communication between users. It enables instant messaging, user authentication, and real-time online/offline status updates. Built with **HTML, CSS, JavaScript, MySQL, PHP, and XAMPP**, the app ensures secure and efficient messaging.

## Features
- **User Authentication:** Secure login and registration system.
- **Real-time Messaging:** Instantly send and receive messages.
- **Online/Offline Status Updates:** See whether a user is currently active.
- **End-to-End Encryption:** Ensures secure communication.
- **Responsive UI:** Works across desktop and mobile devices.
- **Database Storage:** Messages and user data stored in MySQL.


## Tech Stack
- **Frontend:** HTML, CSS, JavaScript
- **Backend:** PHP
- **Database:** MySQL
- **Server:** XAMPP (Apache + MySQL + PHP)

## Installation Guide
### Prerequisites
- Install **XAMPP** from [XAMPP Download](https://www.apachefriends.org/download.html)
- Basic knowledge of PHP and MySQL

### Steps to Set Up the Project
1. **Clone the Repository:**
   ```bash
   git clone https://github.com/yourusername/connectify-app.git
   cd connectify-app
   ```
2. **Start XAMPP:**
   - Open the XAMPP Control Panel.
   - Start Apache and MySQL services.
3. **Setup Database:**
   - Open `phpMyAdmin` (`http://localhost/phpmyadmin/`).
   - Create a new database: `connectify_db`.
   - Import `database.sql` from the project.
4. **Configure Backend:**
   - Open `config.php` and update database credentials.
5. **Run the Application:**
   - Open `http://localhost/connectify-app/` in a browser.


## How It Works
1. **User Registration/Login:**
   - Users register and log in securely.
2. **Messaging:**
   - Users can send and receive real-time messages.
3. **Status Updates:**
   - Active users are marked online.
4. **Database Management:**
   - Messages are stored in MySQL and retrieved dynamically.

## Sample PHP Code for Database Connection
```php
<?php
$servername = "localhost";
$username = "root";
$password = "";
$database = "connectify_db";

$conn = new mysqli($servername, $username, $password, $database);
if ($conn->connect_error) {
    die("Connection failed: " . $conn->connect_error);
}
?>
```

