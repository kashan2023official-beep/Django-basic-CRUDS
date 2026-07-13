# Django Book CRUD Application

A simple Django web application for managing a collection of books. This project implements basic CRUD (Create, Read, Update, Delete) operations.

## Features

- **List Books**: View a complete list of all books in the inventory.
- **Add Book**: Create new book entries with details such as name, author, description, and serial number.
- **Edit Book**: Update details of existing books.
- **Delete Book**: Remove a book from the list.

## Technologies Used

- Python
- Django
- HTML/CSS (Templates)

## Models

### Book
The main model used in this application contains the following fields:
- `name`: Character field (max 100) for the book's title.
- `author`: Character field (max 100) for the author's name.
- `description`: Character field (max 400) for a brief description of the book.
- `serial_no`: Integer field for the book's serial number.

## Getting Started

### Prerequisites

Make sure you have Python and Django installed on your system.

```bash
# Verify Python installation
python --version

# Install Django
pip install django
```

### Installation & Setup

1. **Clone the repository:**
   ```bash
   git clone <https://github.com/kashan2023official-beep/Django-basic-CRUDS>
   cd <repository-directory>
   ```

2. **Activate Virtual Environment (Optional but recommended):**
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows use: venv\Scripts\activate
   ```

3. **Navigate to the project directory:**
   ```bash
   cd mysite
   ```

4. **Apply database migrations:**
   ```bash
   python manage.py makemigrations
   python manage.py migrate
   ```

5. **Run the development server:**
   ```bash
   python manage.py runserver
   ```

6. **Access the application:**
   Open your web browser and go to `http://127.0.0.1:8000/` or the corresponding URL for the book list.

## Project Structure

```
mysite/
├── book/                   # Main application for book management
│   ├── migrations/         # Database migrations
│   ├── templates/book/     # HTML templates for rendering views
│   ├── models.py           # Database models definition
│   ├── views.py            # Logic for handling user requests and returning responses
│   └── ...
├── mysite/                 # Django project settings
│   ├── settings.py         # Project configurations
│   ├── urls.py             # URL routing for the project
│   └── ...
└── manage.py               # Command-line utility for administrative tasks
```
