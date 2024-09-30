# Task Master

## Description
Task Master is a simple web application that allows users to create, update, and delete tasks. This project is built using HTML templates with a backend (assumed to be Flask, Django, or similar) to manage tasks. It displays tasks in a table format, along with the date each task was created, and provides links to update or delete tasks.

## Features
- **Add a task**: Enter a task in the input field and submit it to add a new task to the list.
- **View tasks**: A list of tasks is displayed in a table, showing the task's content and the date it was created.
- **Update a task**: Click on the "Update" link next to a task to modify its content.
- **Delete a task**: Click on the "Delete" link next to a task to remove it from the list.

## File Structure
- `base.html`: The base template that other HTML files (like the one provided) will extend.
- `index.html`: The main HTML template for displaying and managing tasks.
- `update.html`: update HTML file to edit task name.
- `requirements.txt`: This file contains a list of dependencies required for running the project.


## HTML Template Breakdown
- The `Task Master` page extends the base layout (`base.html`) and includes a custom title in the `<head>`.
- Inside the `body`, a task list is shown, or a message indicates there are no tasks.
- A form is provided to add new tasks, and each task can be updated or deleted using links.
  
## Variables
- `tasks`: A list of task objects passed from the backend, each containing:
  - `content`: The description of the task.
  - `date_created`: The date and time when the task was created.
  - `id`: The unique identifier for each task.

## Usage
1. Add tasks using the input field.
2. View the list of tasks in the table.
3. Update or delete tasks by clicking the respective links.

## Installation and Setup
To run this project, follow these steps:
1. Clone this repository.
2. Ensure you have a web framework like Flask or Django installed.
3. Set up the backend to handle routes for adding, updating, and deleting tasks.
   - For example:
     - `/`: Handles adding tasks and displays the list of tasks.
     - `/delete/<id>`: Handles deleting a task with the given `id`.
     - `/update/<id>`: Handles updating a task with the given `id`.
4. Start your server and access the project in your browser.


