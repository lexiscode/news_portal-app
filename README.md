<p align="center"><a href="https://laravel.com" target="_blank"><img src="https://raw.githubusercontent.com/laravel/art/master/logo-lockup/5%20SVG/2%20CMYK/1%20Full%20Color/laravel-logolockup-cmyk-red.svg" width="400" alt="Laravel Logo"></a></p>


# News Portal

Welcome to the News Website Laravel Project! This web application is built using the Laravel framework to provide a platform for publishing and consuming news articles. Whether you're a journalist, an editor, or a reader, this project aims to deliver a seamless and user-friendly experience.

## Features

### User Authentication
- Register: Users can create accounts to personalize their experience.
- Login/Logout: Secure authentication system for user login and logout.

### Article Management
- Create: Authors can create and publish news articles with ease.
- Edit/Update: Authors have the ability to modify and update their published articles.
- Delete: Unwanted articles can be removed from the system.

### Categories
- Categorization: Articles are organized into different categories for easy navigation.
- Create/Edit/Delete Categories: Admins have the power to manage categories.

### User Roles/Permissions
- Admin: Full control over articles, categories, and users.
- Author: Can create, edit, and delete their own articles.
- Reader: Access to browse and read articles.

### Responsive Design 
- Mobile Friendly: The website is designed to work seamlessly on various devices.

### Middleware
- Security features to control access:
    - Certain pages are restricted to non-logged-in users.
    - Specific pages are restricted to logged-in users.

### Search
- Use the search bar to find news articles quickly.

## Getting Started

### Prerequisites
- Make sure you have PHP and Composer installed.
- You need Node.js and npm to handle frontend dependencies. BUT, alternatively, I will highly recommend you download [laragon](https://laragon.org/download/index.html) web server - which has the following pre-installed (Apache 2.4, Nginx, MySQL 8, PHP 8, Redis, Memcached, Node.js 18, npm, git).

### Installation
1. Immediately after installing [laragon](https://laragon.org/download/index.html) web server for the first time, you will need to reboot your computer afterwards.
2. Now into your computer's root directory (e.g. C:), enter these path `C:/laragon/`. Then double-click on the laragon application icon to open it.
3. Now ensure that you have no other web server running (e.g. XAMMP or any other), then inside the Laragon application click on  `StartAll`. Do not stop the server.
4. Then enter into this path directory `C:/laragon/www`, now run this command in order to install Laravel globally `composer global require laravel/installer` 
5. Now git clone this repository still inside this path directory (`C:/laragon/www`): `git clone https://github.com/lexiscode/news_portal-app.git`
6. Next, still in that Laragon application, click on `Database` button (another GUI displays), ensure the Network Type is: `MariaDB or MySQL (TCP/IP)`, if so then click on the `Open` button below the GUI to access the database interface.
7. Now at the top-left corner of the application, you should see `Laragon.MySQL` database section; right-click on it, then select `Create new`, then click on `Database`. Please ensure you name the database `news_portal`, then click OK.
8. Next, open the project directory (`C:/laragon/www/news_portal-app`) with any IDE (e.g. VS Code) and locate a file named `.env.example`, rename the file to `.env` only. 
9. Then inside that same .env file, find and renamed the value of the DB_DATABASE from `DB_DATABASE=news_portal` to `DB_DATABASE=news_portal`
10. Open/Copy/Import the database.sql file query codes inside the database you've created in the Laragon
11. Then still inside the project directory (that is, `C:/laragon/www/news_portal-app`) run this command: `composer install`
12. Lastly, run this migration command, still from within the project directory: `php artisan migrate`
13. Next, generate your own APP_KEY by running this command still from within the project directory: `php artisan key:generate`

Congratulations!!! Now read its Usage documentation below.


## Usage

To use the Personal Task Manager Application, follow these steps:

Open your browser, enter this URL: `http://news_portal-app.test/` OR alternatively, return back to the actual Laragon application GUI, and "right-click" anywhere around its blank body (not a button), select `www` and lastly click on the project name `news_portal-app`.

## Technologies

The Personal Task Manager Application is built using the following technologies:

- **PHP**: A server-side scripting language used for handling data and rendering views.
- **Laravel**: A free and open-source PHP web framework, intended for the development of web applications following the model–view–controller architectural pattern and based on Symfony.
- **MySQL**: A database-based storage system used to store product records.
- **HTML**: A standard markup language for documents designed to be displayed in a web browser. 
- **CSS**: A frontend styling language used to create appealing visuals for the HTML documents.
- **Bootstrap**: A front-end framework that facilitates responsive and modern user interface design.
- **JavaScript**: A powerful programming language used to add interactivity and dynamic behavior to the website.
-- **jQuery**: A JavaScript library designed to simplify HTML DOM tree traversal and manipulation, as well as event handling, CSS animation, and Ajax.

## Contributing

Contributions to the project are welcome! If you encounter any issues or have suggestions for improvements, please open an issue or submit a pull request.

## License

The Laravel framework is open-sourced software licensed under the [MIT license](https://opensource.org/licenses/MIT).
