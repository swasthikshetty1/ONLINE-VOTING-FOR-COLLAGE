
Online Voting System

An Online Voting System built using PHP and MySQL that allows users (voters) to register, log in, and vote for candidates in an election. Admins can manage users, view results, and control the election process. This project is suitable for academic purposes, demonstrations, or small-scale voting systems.


---

Features

For Voters

Registration and secure login

Password encryption using MD5 (can be upgraded to password_hash())

View candidate list

Vote once per election

View confirmation after voting


For Admins

Admin dashboard

Add/edit/delete candidates

View registered users

View voting results

Secure login panel



---

Technologies Used

Frontend

HTML5

CSS3

JavaScript

Bootstrap (or a custom layout)

Font Awesome icons


Backend

PHP (Procedural)

MySQL (via MySQLi)

Sessions for authentication
nstallation Requirements

Software

XAMPP (recommended) or WAMP

PHP 7.0+ (MySQLi required)

MySQL Server

Web browser (Chrome, Firefox, etc.)


Steps to Run

1. Download or Clone the Repository

git clone --  https://github.com/swasthikshetty1/ONLINE-VOTING-FOR-COLLAGE.git


2. Move Project to XAMPP Directory

Copy the project folder (ovs/) to:
C:\xampp\htdocs\



3. Start XAMPP

Open the XAMPP Control Panel.

Start Apache and MySQL.



4. Create the Database

Visit http://localhost/phpmyadmin/

Create a new database named VOTING

Import the provided .sql file (poll.sql) into the database.



5. Edit Database Connection (if needed)

File: connection.php

Update with your MySQL credentials (default is usually root with no password):

$conn = mysqli_connect("localhost", "root", "", "poll");








---

Security Notes

Uses md5() for password encryption — not suitable for production.

Lacks CSRF/XSS protection — suitable for academic use only.

Replace md5() with password_hash() and use prepared statements for enhanced security.

Input sanitization using mysqli_real_escape_string().



---

Future Improvements

Use password_hash() and password_verify() for secure password handling

Implement token-based voting

Add CAPTCHA on login/registration

Responsive design improvements

Admin analytics dashboard

Voter email confirmation



---

Credits

Template by: OS Templates (for front-end layout)



