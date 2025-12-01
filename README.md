# Study Bud

> A community-driven platform for connecting users in study groups. This project is built with **Django** and features real-time activity feeds, dedicated topic rooms, and user profiles. It follows the **Model-View-Template (MVT)** architectural pattern.

## Features

* **Core CRUD Functionality:** Ability to create, read, update, and delete topic rooms.
* **Dynamic Routing:** Uses Django's URL configuration to display unique room pages based on their ID/Primary Key (PK).
* **Template Inheritance:** Implemented a base layout (`main.html`) for consistent navigation and structure across all pages.
* **Database Integration:** Initialized with **SQLite** and includes the core **Room** data model.

## Installation

Follow these steps to get the Django web application running locally.

### Prerequisites

* **Python 3** (version 3.6 or higher)
* **pip** (Python package installer)

### Setup

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/JanelleNYP/studybud.git](https://github.com/JanelleNYP/studybud.git)
    cd studybud
    ```

2.  **Create and activate a virtual environment:**
    This isolates the project dependencies from other Python projects.
    ```bash
    python -m venv venv
    source venv/bin/activate  # On macOS/Linux
    # venv\Scripts\activate   # On Windows
    ```

3.  **Install dependencies:**
    The project only requires Django at this stage.
    ```bash
    pip install django
    # (If a requirements.txt file exists) pip install -r requirements.txt
    ```

4.  **Run Migrations:**
    Apply the initial database schema (including the built-in Django User and Session models) to the `db.sqlite3` file.
    ```bash
    python manage.py migrate
    ```

5.  **Run the Development Server:**
    ```bash
    python manage.py runserver
    ```

## How to Use

Once the server is running, navigate to **`http://127.0.0.1:8000/`** in your web browser.

* The root page displays a list of available rooms (using the views defined in `base/views.py`).
* Clicking a room link will take you to its unique URL (e.g., `/room/1/`).


## Contact

Name - [@JanelleNYP]

Project Link: [https://github.com/JanelleNYP/studybud](https://github.com/JanelleNYP/studybud)