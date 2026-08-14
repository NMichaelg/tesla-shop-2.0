# Tesla-Shop 2.0

A PHP-based e-commerce website developed as a web programming project. The application provides a simple online shopping interface with product browsing, user authentication, product management, and individual product pages.

> **Note:** This project is intended primarily for educational purposes.

## Features

* 🏠 **Home page** with a product-focused storefront
* 🛍️ **Product listing** for browsing available products
* 🔎 **Product details** with individual product pages
* 👤 **User registration** and login
* 🔐 **User logout** functionality
* ➕ **Add products** through the product management interface
* ✏️ **Edit products**
* 🗑️ **Delete products**
* 📩 **Contact page**
* 📱 Responsive styling using Bootstrap
* 🗄️ Product data managed through a database

The application uses a simple page-routing system in `index.php` to load different sections of the website, including the home page, products, authentication pages, and product-management pages.

## Tech Stack

| Technology              | Purpose                       |
| ----------------------- | ----------------------------- |
| **PHP**                 | Server-side application logic |
| **HTML5**               | Page structure                |
| **CSS3**                | Custom styling                |
| **Bootstrap 3**         | Responsive UI components      |
| **JavaScript / jQuery** | Client-side functionality     |
| **MySQL**               | Product and user data storage |

## Project Structure

```text
final_web_lab/
│
├── db_exercise/              # Database-related exercises/files
├── images/                   # Website images and assets
├── pages/
│   ├── add_product/          # Add product functionality
│   ├── contact/              # Contact page
│   ├── delete_product/       # Delete product functionality
│   ├── edit_product/         # Edit product functionality
│   ├── login/                # User login
│   ├── product_list/         # Product listing
│   └── sign_up/              # User registration
│
├── ultis/                    # Utility files
│
├── each_product.php          # Individual product page
├── home.php                  # Home page
├── index.php                 # Main application entry point/router
├── style.css                 # Custom website styles
├── product_database.png      # Database reference/image
├── LICENSE                   # MIT License
└── README.md                 # Project documentation
```

The current repository structure contains separate page directories for adding, editing, and deleting products, as well as login, registration, contact, and product-list functionality.

## Getting Started

### Prerequisites

Before running the project, make sure you have the following installed:

* PHP 7.x or newer
* MySQL / MariaDB
* Apache or another PHP-compatible web server
* A web browser
* Git

For an easy local setup, you can use:

* XAMPP
* WAMP
* MAMP
* Laragon

### 1. Clone the repository

```bash
git clone https://github.com/NMichaelg/final_web_lab.git
cd final_web_lab
```

### 2. Set up the web server

Place the project inside your web server's document root.

For example, with XAMPP:

```text
C:\xampp\htdocs\final_web_lab
```

Then start:

* Apache
* MySQL

### 3. Set up the database

Create a MySQL database for the application and import the project's database structure/data.

The repository includes database-related materials and a `product_database.png` file that can be used as a reference for the product database structure.

> Make sure the database credentials used by the PHP files match your local MySQL configuration.

### 4. Start the application

After starting Apache and MySQL, open:

```text
http://localhost/final_web_lab/
```

The application will load `index.php`, which acts as the main entry point and routes requests to the appropriate pages.

## Application Pages

The application supports several routes through the `page` query parameter:

```text
?page=home
?page=products
?page=contact
?page=login
?page=sign_up
?page=add_product
?page=edit_product
?page=del_product
```

Individual products can also be accessed using an `id` parameter:

```text
?id=<product_id>
```

The routing logic and page inclusions are implemented in `index.php`.

## Product Management

The application provides a basic CRUD workflow for products:

* **Create** — Add a new product
* **Read** — Browse products and view individual product details
* **Update** — Edit existing product information
* **Delete** — Remove products

The product management functionality is organized into separate directories under `pages/`, making each operation easier to maintain.

## User Authentication

Users can create an account through the **Sign Up** page and authenticate through the **Login** page.

After logging in, the application provides access to additional functionality such as product management. Logout functionality is handled through the main application router.

## UI and Styling

The project uses **Bootstrap 3.4.1** alongside a custom `style.css` stylesheet. Bootstrap and jQuery are loaded from CDNs in the main application page.

The interface includes:

* Navigation bar
* Product navigation
* Product listings
* Product details
* Forms
* Authentication pages
* Footer/contact information

## Screenshots / Demo

Add screenshots or a GIF of the application here.

For example:

```markdown
### Home Page

![Home Page](images/home.png)

### Product Page

![Product Page](images/product.png)
```

A demo video is also included in the repository:

```text
2024-11-20 14-25-05.mp4
```

## Known Limitations

This project is a student/educational web application and may require additional configuration depending on the local development environment.

Potential areas for future improvement include:

* Improved authentication and session management
* Stronger input validation
* Password hashing and secure credential storage
* Better authorization for administrative operations
* Improved error handling
* Database configuration through environment variables
* More responsive/mobile-friendly UI
* Shopping cart and checkout functionality
* Automated testing
* Improved accessibility

## Future Improvements

Possible future features include:

* 🛒 Shopping cart
* 💳 Checkout and payment integration
* 📦 Order management
* ⭐ Product reviews and ratings
* 🔍 Product search and filtering
* 📊 Admin dashboard
* 🖼️ Improved product image management
* 👤 User profile management
* 📱 Improved mobile experience

## License

This project is licensed under the **MIT License**.

See [`LICENSE`](LICENSE) for the complete license text.

## Author

**Michael Ng**

GitHub: [NMichaelg](https://github.com/NMichaelg)
