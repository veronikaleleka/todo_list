🚀 Daily Task Manager

A web application for managing daily work. Create tasks, tag them, track their progress from *Not started* to *Completed*, and see a summary of your workload on one dashboard.

Built with Python, Django, and SQLite.

## Features

- **User accounts:** Register, log in, and log out. Each user manages their own tasks.
- **Task management (CRUD):** Create, view, edit, and delete tasks.
- **Status tracking:** Every task has one of three statuses: *Not started*, *In progress*, or *Completed*. Completed tasks are struck through in the list.
- **Tags:** Label tasks with categories such as *Work*, *Studies*, *Home*, or *Workout*. A task can have several tags.
- **Dashboard:** Summary cards show how many tasks are not started, in progress, and completed, plus a count of active tasks.
- **Dates:** Each task has a date, shown in the task list.

## Tech Stack

- **Backend:** Python, Django
- **Frontend:** HTML, CSS, Bootstrap
- **Database:** SQLite (the default Django database, no extra setup needed)
- **Forms:** Django Crispy Forms

## Installation

Requires Python 3.14 or newer.

1. **Clone the repository**

   ```bash
   git clone https://github.com/veronikaleleka/todo_list.git
   cd todo_list
   ```

2. **Create and activate a virtual environment**

   macOS / Linux:
   ```bash
   python3 -m venv .venv
   source .venv/bin/activate
   ```

   Windows:
   ```bash
   python -m venv .venv
   .venv\Scripts\activate
   ```

3. **Install the dependencies** (from the `todo_list` folder)

   ```bash
   pip install -r requirements.txt
   ```

4. **Go to the Django project folder**

   ```bash
   cd mysite
   ```

5. **Apply the database migrations**

   ```bash
   python manage.py migrate
   ```

6. **(Optional) Create an admin account**

   ```bash
   python manage.py createsuperuser
   ```

7. **Start the development server**

   ```bash
   python manage.py runserver
   ```

   Then open http://127.0.0.1:8000 in your browser.

## How to Use

1. Click **Register** and create an account, or **Login** if you already have one.
2. Click **+New Task** and enter a title, a date, a status, and optional tags.
3. Use the blue pencil button to edit a task, or the red bin button to delete it.
4. Change a task's status to *In progress* or *Completed* as you work. Completed tasks are struck through in the list.
5. Check the summary cards at the top of the page to see how much work is left.


## Project Structure

```
todo_list/
├── requirements.txt
└── mysite/          # Django project (run manage.py from here)
    ├── manage.py
    ├── mysite/      # Project settings
    └── todo/        # Main app: models, views, templates
```

---

Made with Django as a learning project.
