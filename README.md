# Django MySQL Portfolio

This project demonstrates how to connect a Django application to a MySQL database. The project includes a simple setup with one application and basic configurations.

## Project Structure

myproject/
├── myapp/
│ ├── init.py
│ ├── admin.py
│ ├── apps.py
│ ├── migrations/
│ ├── models.py
│ ├── tests.py
│ └── views.py
├── myproject/
│ ├── init.py
│ ├── asgi.py
│ ├── settings.py
│ ├── urls.py
│ └── wsgi.py
├── db.sqlite3
├── manage.py
└── Pipfile



## Prerequisites

- Python 3.9 or higher
- MySQL server
- pipenv for managing the virtual environment

## Setup Instructions

1. **Clone the repository:**

    ```bash
    git clone https://github.com/artafarshadi1996/django-mysql-portfolio.git
    cd django-mysql-portfolio
    ```

2. **Create and activate the virtual environment:**

    ```bash
    pip install pipenv
    pipenv install
    pipenv shell
    ```

3. **Update the database configuration:**

    Open `myproject/settings.py` and update the `DATABASES` dictionary with your MySQL credentials:

    ```python
    DATABASES = {
        'default': {
            'ENGINE': 'django.db.backends.mysql',
            'NAME': 'your_database_name',
            'USER': 'your_database_user',
            'PASSWORD': 'your_database_password',
            'HOST': 'localhost',
            'PORT': '3306',
        }
    }
    ```

4. **Run migrations:**

    ```bash
    python manage.py makemigrations
    python manage.py migrate
    ```

5. **Run the development server:**

    ```bash
    python manage.py runserver
    ```

6. **Open your browser:**

    Navigate to `http://127.0.0.1:8000` to see the Django welcome page.

## Usage

- This project serves as a starting point for connecting Django to MySQL. 
- Customize the models in `myapp/models.py` to define your database schema.
- Create views in `myapp/views.py` and map them in `myapp/urls.py`.

## Contributing

Contributions are welcome! Please fork the repository and submit a pull request with your changes.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Contact

For any inquiries, please contact the repository owner.

Instructions to Add and Push the README.md File
Create the README.md file:

In your project directory, create a new file named README.md and paste the above content into it.
Add the README.md file to Git:

bash
Copy code
git add README.md
Commit the changes:

bash
Copy code
git commit -m "Add project README"
Push to GitHub:

bash
Copy code
git push origin main
