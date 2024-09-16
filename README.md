# Flask Blog Website

A feature-rich blog website built with Flask, offering user authentication, blog post management, and commenting functionality.

## Features

### User Authentication
- User registration with email, name, and password
- Secure password hashing using Werkzeug's security features
- User login and logout functionality
- Flask-Login integration for user session management

### Blog Post Management
- Create, read, update, and delete (CRUD) operations for blog posts
- Rich text editing for blog post content using CKEditor
- Blog posts include title, subtitle, body content, and featured image URL
- Date stamping for blog posts

### User Roles
- Admin user with special privileges (user with ID 1)
- Admin-only access to create, edit, and delete blog posts

### Commenting System
- Authenticated users can comment on blog posts
- Comments are associated with both the user and the blog post

### User Profiles
- Gravatar integration for user profile pictures

### Responsive Design
- Bootstrap 5 integration for a mobile-friendly, responsive layout

### Security Features
- CSRF protection for all forms
- Environment variable usage for sensitive information (e.g., secret keys, database URIs)

### Database
- SQLAlchemy ORM for database operations
- Flexible database backend (SQLite for development, easily adaptable for production databases)

### Additional Pages
- About page
- Contact page (with optional email functionality)

## Technical Stack

- **Backend**: Flask (Python)
- **Database**: SQLAlchemy with SQLite (configurable for other databases)
- **Frontend**: HTML, CSS, JavaScript
- **CSS Framework**: Bootstrap 5
- **Forms**: Flask-WTF and WTForms
- **Authentication**: Flask-Login
- **Text Editor**: CKEditor
- **Profile Pictures**: Gravatar

## Setup and Installation

1. Clone the repository
2. Create a virtual environment and activate it
3. Install dependencies: `pip install -r requirements.txt`
4. Set up environment variables in a `.env` file:
   ```
   FLASK_KEY=your_secret_key
   DB_URI=your_database_uri
   ```
5. Initialize the database: `flask db upgrade`
6. Run the application: `flask run`

## Usage

- Navigate to `http://localhost:5000` in your web browser
- Register a new account or log in
- Explore blog posts, create new posts (if admin), or leave comments

## Development

- Debug mode can be enabled by setting `debug=True` in `app.run()`
- For production deployment, ensure to use a production-ready WSGI server

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.


