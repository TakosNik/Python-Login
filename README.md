# Python-Login
A python login and register project with html and mysql.


main.py: this is the main project file, as I do this to practice back end with Python.
index.html: Login form created with HTML5 and CSS3.
register.html: Registration form created with HTML5 and CSS3.
home.html: The home template is what logged-in users will see.
profile.html: The profile template display for logged-in users.
layout.html The layout template for the home and profile templates.
style.css The CSS3 stylesheet for our login and registration system.

Database query for the project with user test:

CREATE DATABASE IF NOT EXISTS `pythonlogin` DEFAULT CHARACTER SET utf8 COLLATE utf8_general_ci;
USE `pythonlogin`;

CREATE TABLE IF NOT EXISTS `accounts` (
	`id` int(11) NOT NULL AUTO_INCREMENT,
  	`username` varchar(50) NOT NULL,
  	`password` varchar(255) NOT NULL,
  	`email` varchar(100) NOT NULL,
    PRIMARY KEY (`id`)
) ENGINE=InnoDB AUTO_INCREMENT=2 DEFAULT CHARSET=utf8;

INSERT INTO `accounts` (`id`, `username`, `password`, `email`) VALUES (1, 'test', 'test', 'test@test.com');