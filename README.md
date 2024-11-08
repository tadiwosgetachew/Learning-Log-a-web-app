# Learning Log

Welcome to **Learning Log**! This is a simple Django-based web application where learners can record and track what they’ve learned. Whether you're learning programming, languages, or any other subject, this app allows you to jot down notes and keep track of your progress.

## Features
- **Log entries**: Create, read, update, and delete notes on what you've learned.
- **Categorized notes**: Organize entries by topics for easy reference.
- **User authentication**: Sign up and log in to access and manage your learning logs.
- **Responsive design**: Works well on both desktop and mobile devices.

## Table of Contents

- [Installation](#installation)
- [Usage](#usage)
- [Development](#development)
- [Contributing](#contributing)
- [Acknowledgments](#acknowledgments)

## Installation

To run the Learning Log project locally, follow these steps:

### Prerequisites

- **Python 3**: Make sure Python 3 is installed on your machine. You can download it from [python.org](https://www.python.org/downloads/).

### Step 1: Clone the Repository

Clone the project repository to your local machine:

```bash
git clone https://github.com/tadiwosgetachew/Learning-Log-a-web-app.git
```

### Step 2: Set Up a Virtual Environment

Create and activate a virtual environment to isolate your project dependencies:

```bash
# For Mac/Linux:
python3 -m venv venv
source venv/bin/activate

# For Windows:
python -m venv venv
ll_env\Scripts\activate
```

### Step 3: Install Dependencies

Install the required Python dependencies using `pip`:

```bash
pip install -r requirements.txt
```

### Step 4: Set Up the Database

Run the following command to set up the database (SQLite by default):

```bash
python manage.py migrate
```

### Step 5: Create a Superuser (Optional)

To access the Django admin interface, create a superuser:

```bash
python manage.py createsuperuser
```

Follow the prompts to create an admin account.

### Step 6: Run the Server

Start the Django development server:

```bash
python manage.py runserver
```

Once the server is running, you can open your browser and go to [http://127.0.0.1:8000/](http://127.0.0.1:8000/) to use the app locally.

## Usage

### Accessing the App

- After running the development server, you can visit [http://127.0.0.1:8000/](http://127.0.0.1:8000/) to start using the Learning Log app.
- Sign up for an account, or log in if you already have one.
- Create and manage your learning logs, categorize them by topics, and view all your previous entries.

### Admin Interface

- To access the Django admin interface, go to [http://127.0.0.1:8000/admin](http://127.0.0.1:8000/admin).
- Use the superuser account created earlier to log in and manage users, logs, and categories.

## Development

### Cloning the Repository

Clone the repository if you haven't done so already:

```bash
git clone https://github.com/tadiwosgetachew/Learning-Log-a-web-app.git
```

### Installing Dependencies

Ensure you have all the necessary dependencies installed:

```bash
pip install -r requirements.txt
```

### Configure the `.env` File

In the project root (same level as `manage.py`), create a file called `.env` and open it in a text editor. Add the following settings to the file:

```env
# Secret key for cryptographic signing
SECRET_KEY=your-generated-secret-key  # You can generate one at the Django Secret Key Generator (https://djecrety.ir/)

# Set to 'True' for development, 'False' for production
DEBUG=True

# Database URL for local development (SQLite is fine for testing)
DATABASE_URL=sqlite:///db.sqlite3 
```

### Running the Development Server

To run the app locally and test your changes, run:

```bash
python manage.py runserver
```

### Running Tests

You can run Django's built-in tests to make sure everything is working as expected:

```bash
python manage.py test
```

## Contributing

contributions to the Learning Log project is welcome!

1. **Fork the repository**.
2. **Create a new branch** for your feature or bug fix:
   ```bash
   git checkout -b my-feature-branch
   ```
3. **Make your changes**, and commit them:
   ```bash
   git commit -m "Add new feature"
   ```
4. **Push your changes** to your fork:
   ```bash
   git push origin my-feature-branch
   ```
5. **Create a pull request** from your forked repo to the main project.


## Acknowledgments

- **Django**: The framework used to build this app.
- **Bootstrap 3**: For styling the frontend of the application.
- **python-dotenv**: For environment variable management.



