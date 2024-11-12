# **Zoomies** Blog

A full-featured blog built with Flask for REST API implementation, SQLAlchemy for database management, and Bootstrap for a clean, responsive UI.

**Live Demo**: [https://zoomies-io.onrender.com](https://zoomies-io.onrender.com)

---

## Features

- **REST API**: Built with Flask, following RESTful principles for modular, scalable code.
- **Database Management**: SQLAlchemy ORM retrieves posts and comments from a PostgreSQL database.
- **Rich Text Editing**: Integrated with `flask_ckeditor` to allow easy post and comment formatting.
- **User Authentication**: Password security implemented with Werkzeug, including salted hashing.
- **Admin Capabilities**: allow editing/deleting any posts and comments.
- **Post Management**: Users can create, edit, and delete posts and comments with `WTForms`.
- **Modern UI**: Built with Bootstrap for a responsive and clean user experience.
- **Deployment**: Hosted on Render.com for easy accessibility.

## Project Setup

### Prerequisites

- Python 3.x
- A live database supported by SQLAlchemy
- Dependencies in `requirements.txt`

### Installation

1. **Clone the repository**:
   ```bash
   git clone https://github.com/muhzinkhan/blog.git
   cd blog
   ```

2. **Install dependencies**:
   ```bash
   pip install -r requirements.txt
   ```

3. **Configure the Database**:
   - Create a any database supported by SQLAlchemy.
   - Create the `DB_URI` variable in the `.env` file with your database credentials.

4. **Configure email for contact**:
   - Create the `OWN_EMAIL` and `OWN_PASSWORD` variables in the `.env` file.

5. **Setup Flask app**:
   - Create the `FLASK_SECRET_KEY` variable in the `.env` file for the Flask application.

6. **Run the Application**:
   ```bash
   python3 main.py
   ```

## Usage

- **Navigate to** your localhost to view the blog.
- **Register/Login** to start creating and managing posts.
- First user to regester will be the **admin** (allow posting/editing/deleting any posts) while **other users** will only be able to comment and **guests** can only perform the action of viewing posts.
- **Note**: This application is ready for production and works well with `gunicorn`.