# Local Library Website

The Local Library Website is a web application built using Django that serves as an online catalog for a local library. It allows users to browse, search, and check out books, as well as view information about authors and genres. This README provides an overview of the project, its features, and instructions for running and deploying the application.

## Features

- **Browse Catalog**: Users can view a list of all available books in the library.
- **Search**: Users can search for books by title, author, genre, or keyword.
- **Book Detail Page**: Clicking on a book displays detailed information about the book, including its availability.
- **Author Information**: Users can view information about authors and see a list of books written by each author.
- **Genre Information**: Users can explore books by genre and see a list of books in each genre.
- **User Authentication**: Users can create accounts, log in, and borrow books.
- **Admin Panel**: Administrators can manage books, authors, genres, and user accounts through the Django admin panel.
- **Borrow and Return**: Users can borrow and return books, with due dates and notifications for overdue books.
- **Responsive Design**: The website is responsive and can be accessed from various devices.


## Usage

1. **Visit the website**: Open your web browser and navigate to [http://localhost:8000/](http://localhost:8000/).

2. **Browse the catalog**: Explore the library's catalog by browsing through the list of available books.

3. **Search for books**: Use the search feature to find books by title, author, genre, or keywords.

4. **View book details**: Click on a book to view detailed information, including its title, author, genre, and availability status.

5. **Create a user account**: If you're a new user, you can create an account by clicking on the "Sign Up" option. Provide your details and create a username and password.

6. **Log in**: For existing users, log in using your username and password.

7. **Borrow books**: Once logged in, you can borrow books by clicking the "Borrow" button on a book's detail page. The due date for borrowed books will be displayed.

8. **Return books**: Return borrowed books before or on the due date to avoid overdue notifications.

9. **Explore authors and genres**: Discover more books by exploring author profiles and genre categories.

10. **Admin Panel**: As an administrator, you can access the admin panel by visiting [http://localhost:8000/admin/](http://localhost:8000/admin/). Use your admin credentials to manage books, authors, genres, and user accounts.

## Database

The Local Library Website uses Django's default SQLite database for development. In a production environment, you may consider using a more robust database system such as PostgreSQL or MySQL.

To set up a different database, update the database settings in the `settings.py` file.

```python
DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.sqlite3',
        'NAME': BASE_DIR / 'db.sqlite3',
    }
}