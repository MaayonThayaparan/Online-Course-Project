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
          - If prompted to 'Please select a fix', select option '1-Provide a one-odd default now...'
          - Enter an integer value
     - python manage.py migrate
     - python manage.py runserver
- Last commmand will run the server. Open web browser and enter URL: http://localhost:8000/onlinecourse

- Without being logged in, you can do the following:
     - View courses available
     - Open course to view lessons
     - ![image](https://github.com/MaayonThayaparan/Online-Course-Project/assets/43158629/3647724d-51ff-4777-bbc4-f074c85a3418)

- Sign Up as new user.
     - Click the 'Sign Up' button in the top right.
     - Input values for all fields and click 'Sign Up'
     - ![image](https://github.com/MaayonThayaparan/Online-Course-Project/assets/43158629/638781cb-e090-4118-b147-8fdd92b01e61)
     - You are now signed in. You can logout by clicking the 'Logout' button.
     - ![image](https://github.com/MaayonThayaparan/Online-Course-Project/assets/43158629/926022ad-ba4c-42ca-bf3d-21e9816bb2f5)

- Authorized user, you can do the following:
     - View courses available
     - Enroll for a course (this will increase the enroll counter on the course when you hit 'Enroll')
     - Open course to view lesson
     - To can take the exam for the course by clicking on 'Start Exam'
     - ![image](https://github.com/MaayonThayaparan/Online-Course-Project/assets/43158629/bdd3f0b5-a577-4c29-ba0f-fab43ac605ce)
     - Make your selections and click 'Submit' to complete exam
     - ![image](https://github.com/MaayonThayaparan/Online-Course-Project/assets/43158629/ccd912f8-9fbc-480c-be68-250ba34a1ab4)
     - If you fail the exam, you can click 'Re-test' to redo the exam
     - ![image](https://github.com/MaayonThayaparan/Online-Course-Project/assets/43158629/9d4b98f8-72c7-4aa0-a1ab-30b31e6a906c)
     - When you pass the exam you will be congratulated:
     - ![image](https://github.com/MaayonThayaparan/Online-Course-Project/assets/43158629/a75ab7eb-6faa-47ca-80e7-b91f14e571b5)

### Customize the Webpage
- Django admin site has been configured for this project.
- You can acces the admin site at: http://localhost:8000/admin
- A superuser has already been created, you can login as an admin using the below credentials:
     - username: root
     - password: root
- If the above superuser does not work, do the following:
     - Stop the server (Ctrl+c in terminal).
     - Run the following command in the project directory in terminal: python manage.py createsuperuser
     - Follow the onscreen prompts.
     - Run the server and login to the admin site using your newly created superuser.
- From the admin site, you can add/delete courses, lessons, questions, choices, instructors, and learners.
- ![image](https://github.com/MaayonThayaparan/Online-Course-Project/assets/43158629/8811bc89-c9e9-4d09-b056-78ab77f79e3b)

- If you want to start from scratch, delete the db.sqlite3 file in the project folder.
- If you are going to change the models, ensure you run the following two commands before restarting the server:
     - python manage.py makemigrations onlinecourse
     - python manage.py migrate


## Future Optimizations
- Change models so there is an exam per lesson, then final exam for whole course. 
- Save the completion status of lessons and courses per user. 



      



          
            

         
      
       



