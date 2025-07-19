# 🌍 AQI Checker

A simple and user-friendly web app to check real-time **Air Quality Index (AQI)** for cities around the world. Perfect for travelers and health-conscious users.

## ✨ Features

- 🔐 **User Auth** – Register, log in, and choose a preferred background color.
- 🏙️ **City Selection** – Select up to 10 cities to monitor.
- 📊 **Live AQI Display** – Get clean, readable AQI tables.
- 🍪 **Saved Preferences** – Background color saved via cookies.
- 💡 **Clean UI** – Designed for simplicity and ease of use.

## 🛠️ Tech Stack

- **PHP** – Backend logic & DB handling  
- **MySQLi** – User & city data storage  
- **HTML5 / CSS3** – Structure & styling  
- **JavaScript** – Form validation & UX

- ## 🖥️ How to Run Locally

Follow these steps to set up and run the AQI Checker on your local machine:

### 1. Clone the Repository

```bash
git clone https://github.com/ss-pranto/Air-Quality-Index.git
cd aqi-checker
```

### 2. Set Up the Database

- Open your MySQL tool (e.g., phpMyAdmin or MySQL CLI).
- Create a new database named `aqi`.
- Create two tables:
  - `user` – to store user credentials and preferences.
  - `info` – to store city, country, and AQI data.
- You can check `process.php` and `request.php` for the required table structure.

### 3. Configure Database Connection

Open the following files and update your DB credentials:

- `login.php`
- `process.php`
- `request.php`

Example (default XAMPP settings):

```php
mysqli_connect("localhost", "root", "", "aqi");
```

### 4. Start a Local Web Server

- If you're using **XAMPP**, move the project folder to `htdocs/`.
- Start **Apache** and **MySQL** from the XAMPP Control Panel.

### 5. Open in Browser

Visit the app in your browser:

```
http://localhost/aqi-checker/index.html
```

You should now see the AQI Checker interface and be able to register, log in, and check AQI data.
