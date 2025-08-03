# FastAPI Notes App

A simple Notes web application built with FastAPI, MongoDB, and Jinja2 templates.

---

## Features

- Create and list notes
- Store notes in MongoDB
- Form submission with proper validation
- Jinja2 templating for dynamic HTML pages

---

## Requirements

- Python 3.12+
- MongoDB instance (local or cloud such as Atlas)
- pip packages listed in `requirements.txt`

---

## Setup Instructions

### 1. Clone the repository


### 2. Create and activate a virtual environment


### 3. Install dependencies


### 4. Setup environment variables

Create a `.env` file in the project root directory with your MongoDB connection string:


**Note:** Replace `<username>`, `<password>`, `<cluster-url>`, and `<your-db-name>` with your actual MongoDB cluster details.

---

## Running the Application


- Open a browser and go to [http://127.0.0.1:8000](http://127.0.0.1:8000) to use the app.

---

## Project Structure

- `main.py` - FastAPI app entry point
- `routes/` - API routes including note routes
- `models/` - Pydantic models (if any)
- `schemas/` - MongoDB schema converters (`noteEntity`, etc.)
- `templates/` - Jinja2 HTML templates
- `config/` - MongoDB database connection setup
- `.env` - Environment variables (not committed to GitHub)
- `requirements.txt` - Python dependencies

---

## Important

- Never commit `.env` file or any files that contain your MongoDB credentials.
- Use `.gitignore` to exclude your `.env` and virtual environment folder (`venv/`).
- Make sure to restart the FastAPI server after installing new dependencies.

---

## Troubleshooting

- Form submission errors requiring multipart parsing?  
  Ensure `python-multipart` is installed:
