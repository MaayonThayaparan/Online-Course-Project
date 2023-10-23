# Online Course and Exams

## Description

- This is a Django project which displays online courses. 
- Unregistered users can only view course content.
- Registered users can enroll in courses and take the course exam.
     - Course exam will fail or pass user based on submission details.
- This webpage is fully customizable as an admin (details provided). 

## Getting Started

### Dependencies
- Tested on Windows 10
- Tested on Python 3.12.0
- Download Python from: https://www.python.org/downloads/
- Requires Python packages: Django, Pillow, distro-info, virtualenv, Django psycopg2-binary

### Installation
- Download Python from: https://www.python.org/downloads/
- Download project from GitHub
- Open a new terminal and run following commands:
     - pip install django
     - python -m pip install Pillow
     - pip install --upgrade distro-info
     - pip install virtualenv
     - pip install Django psycopg2-binary
     - pip install aiohttp
     - virtualenv djangoenv
     - source djangoenv/bin/activate
  
### Executing the Program
- Open terminal
- Navigate to the project folder
- Run the following commands:
     - python -m pip install -U -r requirements.txt
     - python manage.py makemigrations onlinecourse
     - python manage.py migrate
     - python manage.py runserver
- Last commmand will run the server. Open web browser and enter URL: http://localhost:8000/onlinecourse


## Future Optimizations
- Connect an actual database that store the data
- Add functionality for 'Edit', 'Delete', 'Comments', 'Category'



      



          
            

         
      
       



