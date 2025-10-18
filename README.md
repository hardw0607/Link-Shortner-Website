A simple PHP-based Link Shortener that converts long URLs into short, shareable links.  
It also supports redirection and QR code generation.

---

## 🚀 Features
- ✂️ Shorten long URLs instantly
- 🔁 Redirect to the original link
- 🧾 Generate QR codes for short links
- 📱 Simple and responsive UI
- ⚙️ Uses `.htaccess` for clean URLs (no query strings)

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
1. **Install** [XAMPP](https://www.apachefriends.org/) or [WAMP](https://www.wampserver.com/).
2. Move the `short` folder to:
   - `htdocs` (for XAMPP)
   - `www` (for WAMP)
3. Open **phpMyAdmin** and create a database named `shortener`.
4. Run the following SQL query:
   ```sql
   CREATE TABLE links (
       id INT AUTO_INCREMENT PRIMARY KEY,
       original_url TEXT NOT NULL,
       short_code VARCHAR(10) NOT NULL UNIQUE,
       created_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP
   );
   ```
5. Start **Apache** and **MySQL** from your control panel.
6. Open your browser and visit:
   ```
   http://localhost/short/
   ```

---

## 🧠 How It Works
1. The user enters a long URL.
2. PHP generates a unique short code and saves it in the database.
3. When the short link is visited, it redirects to the original URL.
4. A QR code can also be generated for easier sharing.

---

## 👨‍💻 Authors
- **Sarvesh Kumar**
- **Peeyush Tripathi**
- **Suraj Vishwakarma**
- **Ishant Shrivastava**

---

## 📄 License
This project is open-source and free to use for educational purposes.
