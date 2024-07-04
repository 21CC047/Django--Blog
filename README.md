Tech & Sports Explainer
This project aims to create a platform where users can upload and manage explanations about various topics, such as technologies and sports. The data is stored in a MySQL database and can be managed through an admin login.

Tech Stack
Frontend: HTML, CSS
Backend: Django (Python)
Database: MySQL (using MySQL Workbench for management)
Features
Admin Login: Secure login for administrators to manage content.
Content Management:
Upload explanations for different topics.
Categorize explanations (e.g., Technology, Sports).
View, edit, and delete existing explanations.
Database Management:
Store and track explanations in a MySQL database.
Installation and Setup
Prerequisites
Python
Django
MySQL
MySQL Workbench
Steps
Clone the repository:

bash
Copy code
git clone https://github.com/your-username/tech-sports-explainer.git
cd tech-sports-explainer
Create a virtual environment and activate it:

bash
Copy code
python -m venv venv
source venv/bin/activate  # On Windows use `venv\Scripts\activate`
Install dependencies:

bash
Copy code
pip install -r requirements.txt
Set up MySQL database:

Create a database using MySQL Workbench.
Update settings.py in your Django project with your database credentials:
python
Copy code
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
Apply migrations:

bash
Copy code
python manage.py migrate
Create a superuser (admin):

bash
Copy code
python manage.py createsuperuser
Run the development server:

bash
Copy code
python manage.py runserver
Access the admin portal:

Go to http://127.0.0.1:8000/admin in your web browser.
Log in using the superuser credentials you created.
Usage
Admin Dashboard: After logging in, you can manage the explanations by adding new ones, editing existing ones, and deleting those that are no longer needed.
Categorization: Ensure explanations are categorized correctly to maintain organization.
Contributing
Feel free to fork this repository, make feature branches, and create pull requests. For major changes, please open an issue first to discuss what you would like to change.
