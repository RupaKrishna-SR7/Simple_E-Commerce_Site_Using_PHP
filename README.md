# Simple E-Commerce Site Using PHP

This is a simple e-commerce web application built using PHP, MySQL, and Bootstrap. The application allows users to browse products, view details, leave feedback, and interact with sellers. Sellers must register and await admin approval before they can post products. The admin is responsible for managing seller accounts, product listings, and user comments.

## Key Features

### 1. User Registration
- **Sellers**: Sellers need to register an account and await admin approval before posting products. Once approved, they can add, update, or delete their product listings.
  
### 2. Product Management
- **Admin Approval**: Products added by sellers must be reviewed and approved by the admin before being displayed on the site.
  
### 3. Interactive Product Pages
- **User Comments**: Users can leave comments on product pages, providing feedback or asking questions.
- **Seller Information**: Users can view detailed information about sellers on product pages.

### 4. Admin Control Panel
- **Seller Management**: The admin can approve, disapprove, or block seller accounts.
- **Product Management**: The admin can approve or disapprove product listings and manage all products on the site.
- **User Feedback Management**: The admin can view and moderate user comments on product pages.

## Prerequisites

Before you begin, ensure you have met the following requirements:
- **PHP** (>= 7.0)
- **MySQL** (>= 5.7)
- A **Web Server** (e.g., Apache) configured to run PHP applications.

## Installation

Follow these steps to get the application up and running:

1. **Clone the Repository**
   ```bash
   git clone https://github.com/RupsKrishna-SR7/simple-ecommerce-site.git
   ```
   Or download the repository as a ZIP file and extract it.

2. **Database Setup**
   - Import the `shop.sql` file into your MySQL server:
     ```sql
     mysql -u username -p database_name < path/to/shop.sql
     ```
   - Update the database configuration in `config.php` with your MySQL credentials.

3. **Serve the Application**
   - Place the `E-Commerce-Site` folder in your web server's root directory (e.g., `htdocs` for XAMPP or `www` for WAMP).
   - Start your web server.

4. **Access the Application**
   - Open your web browser and navigate to `http://localhost/E-Commerce-Site` (or the URL configured on your web server).

## Folder Structure

```
E-Commerce-Site/
│
├── assets/               # Static assets like CSS, JS, and images
├── includes/             # Common files like header, footer, and database connection
├── admin/                # Admin dashboard files
├── seller/               # Seller dashboard and product management files
├── user/                 # User-facing pages like product listings and comments
├── config.php            # Database configuration file
├── index.php             # Homepage of the e-commerce site
├── shop.sql              # SQL file for creating the database schema
└── README.md             # Project documentation
```

## Admin Access

- **Admin URL**: Access the admin panel at `http://localhost/E-Commerce-Site/admin/`.
- **Default Admin Credentials**:
  - **Username**: `admin`
  - **Password**: `admin123` (change this after the first login)

## Troubleshooting

- **Database Connection Issues**: Ensure your `config.php` file has the correct MySQL credentials and that your MySQL server is running.
- **File Permissions**: On some servers, you may need to adjust file permissions to ensure the web server can read/write files.
- **PHP Errors**: Enable error reporting in PHP to debug issues. Add the following to the top of your `index.php` file:
  ```php
  error_reporting(E_ALL);
  ini_set('display_errors', 1);
  ```

## Contributing

If you would like to contribute to this project, please fork the repository and submit a pull request with your improvements. 

## License

This project is open-source and available under the MIT License.
