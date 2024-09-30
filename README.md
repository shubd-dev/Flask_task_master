# Task Master

## Description
Task Master is a simple web application that allows users to create, update, and delete tasks. This project is built using HTML templates with a Flask backend to manage tasks. It displays tasks in a table format, along with the date each task was created, and provides links to update or delete tasks. The data is saved locally in an SQLite database file.

## Features
- **Add a task**: Enter a task in the input field and submit it to add a new task to the list.
- **View tasks**: A list of tasks is displayed in a table, showing the task's content and the date it was created.
- **Update a task**: Click on the "Update" link next to a task to modify its content.
- **Delete a task**: Click on the "Delete" link next to a task to remove it from the list.

## File Structure
- `templates/base.html`: The base template that other HTML files (like `index.html`) will extend.
- `templates/index.html`: The main HTML template for displaying and managing tasks.
- `templates/update.html`: A separate template for editing task content.
- `requirements.txt`: This file contains the list of dependencies required to run the project.
- `instance/todo.db`: SQLite database file where tasks are stored.
- `static/main.css`: CSS file for styling the Task Master application.

## HTML Template Breakdown
- The `Task Master` page extends the base layout (`base.html`) and includes a custom title in the `<head>`.
- Inside the `body`, a task list is shown, or a message indicates there are no tasks.
- A form is provided to add new tasks, and each task can be updated or deleted using links.

## Variables
- `tasks`: A list of task objects passed from the backend, each containing:
  - `content`: The description of the task.
  - `date_created`: The date and time when the task was created.
  - `id`: The unique identifier for each task.

## Installation and Setup

To run this project locally, follow the steps below:

### 1. Clone the repository
First, clone the repository to your local machine:
```bash
git clone https://github.com/your-username/task-master.git
cd task-master
# Create a virtual environment called 'env'
python -m venv env

# Activate the virtual environment
# On Windows:
env\Scripts\activate

# On macOS/Linux:
source env/bin/activate
pip install -r requirements.txt 
python app.py
http://127.0.0.1:5000/



### Instructions Overview:
1. **Clone** the repository.
2. **Set up** a virtual environment called `env` using `python -m venv env`.
3. **Activate** the virtual environment.
4. **Install dependencies** using `pip install -r requirements.txt`.
5. **Run** the Flask server using `python app.py`.
6. **Access** the app at `http://127.0.0.1:5000/`.

Let me know if you'd like any further changes!
