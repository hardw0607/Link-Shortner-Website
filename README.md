# Link-Shortner-Website
# 🔗 Link Shortener Website

A simple PHP-based Link Shortener that converts long URLs into short, shareable links. 
It also supports redirection and QR code generation.

---

## 🚀 Features
- Shorten long URLs instantly
- Redirect to the original link
- Generate QR codes for short links
- Simple and responsive design
- Uses .htaccess for clean URLs

---

## 🛠️ Technologies Used
- PHP
- MySQL
- HTML, CSS
- Apache Server (XAMPP / WAMP)

---

## 📂 Folder Structure
```
short/
├── index.html
├── shorten.php
├── redirect.php
├── api.php
├── qr.php
├── styles2.css
└── .htaccess
```

---

## ⚙️ Setup Instructions
1. Install XAMPP or WAMP.
2. Move the `short` folder to:
   - `htdocs` (for XAMPP)
   - `www` (for WAMP)
3. Create a database named `shortener` in phpMyAdmin.
4. Run this SQL query:
   ```sql
   CREATE TABLE links (
       id INT AUTO_INCREMENT PRIMARY KEY,
       original_url TEXT NOT NULL,
       short_code VARCHAR(10) NOT NULL UNIQUE,
       created_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP
   );
   ```
5. Start Apache and MySQL.
6. Open your browser and go to:
   ```
   http://localhost/short/
   ```

---

## 🧠 How It Works
- User enters a long URL.
- PHP generates a short code and saves it in the database.
- When someone visits the short link, it redirects to the original URL.
- QR codes can also be generated for each short link.

---

## 👨‍💻 Authors
- **Sarvesh Kumar**
- **Peeyush Tripathi**  
- **Suraj Vishwakarma**  
- **Ishant Shrivastava**  

