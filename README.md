py -m venv venv

2. Activate the Virtual Environment

Windows:

.\venv\Scripts\activate

Linux / MacOS:

source venv/bin/activate



3. Install Required Packages

Install Django, django-environ, and MySQL client:

pip install django
pip install django-environ
pip install psycopg2-binary



4. Configure .env File

Create a .env file in the project root (you can copy .env.example):

SECRET_KEY=your-secret-key-here
DEBUG=True
NAME=your-database-name
USER=your-database-username
PASSWORD=your-database-password
HOST=localhost
PORT=5432


6. Run the Project
python manage.py migrate
python manage.py runserver
