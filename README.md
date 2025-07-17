# Library Management System

[![Django CI](https://github.com/yourusername/library-management/actions/workflows/django.yml/badge.svg)](https://github.com/yourusername/library-management/actions/workflows/django.yml)
[![Coverage Status](https://coveralls.io/repos/github/yourusername/library-management/badge.svg?branch=main)](https://coveralls.io/github/yourusername/library-management?branch=main)

A comprehensive library management system built with Django that helps librarians manage books, members, and borrowing operations efficiently.

## 📚 Features

### Core Functionality
- **Book Management**: Add, edit, search, and categorize books
- **Member Management**: Register patrons with contact information
- **Borrowing System**: Track book loans with due dates
- **Fines Calculation**: Automatic late fee calculation
- **Inventory Management**: Track book copies and availability
- **Reporting**: Generate usage statistics and overdue books list

### User Experience
- **Role-based Access**: Separate interfaces for librarians vs. members
- **Responsive Design**: Mobile-friendly with Bootstrap 5
- **Search & Filters**: Find books by title/author/category
- **Notifications**: Email reminders for due dates

### Admin Features
- **Dashboard**: Overview of library operations
- **Fine Management**: View and update patron fines
- **CSV Import**: Bulk import books from spreadsheet
- **Custom Admin**: Enhanced Django admin interface

## 🛠️ Tech Stack
- **Backend**: Django 4.2, Python 3.10
- **Database**: PostgreSQL
- **Frontend**: Bootstrap 5, HTMX
- **Task Queue**: Celery with Redis
- **Deployment**: Docker, Nginx, Gunicorn

## ⚙️ Installation

### Prerequisites
- Python 3.10+
- PostgreSQL 14+
- Redis

### Setup
```bash
# Clone repository
git clone https://github.com/yourusername/library-management.git
cd library-management

# Create virtual environment
python -m venv venv
source venv/bin/activate

# Install dependencies
pip install -r requirements.txt

# Configure environment
cp .env.example .env
# Edit .env with your database credentials

# Apply migrations
python manage.py migrate

# Create superuser
python manage.py createsuperuser

# Run development server
python manage.py runserver
