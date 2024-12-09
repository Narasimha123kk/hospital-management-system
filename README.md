# hospital-management-system

![admin_dashboard](https://github.com/user-attachments/assets/02d89966-62dc-44ef-915e-1db866632af4)
![admin_doctor](https://github.com/user-attachments/assets/e7c95b7b-9fd9-4783-ba79-d82005d588f8)
![homepage](https://github.com/user-attachments/assets/162cfb05-de32-4f5e-a29e-fa2330b1d639)
![invoice](https://github.com/user-attachments/assets/0aee29c0-c267-4224-9a8a-3f9f368f52b1)


System Features
Admin Panel
Account Management:
Can sign up and log in without approval.
Doctor Management:
Register, view, approve, reject, or delete doctors.
Approve doctor applications for jobs at the hospital.
Patient Management:
Admit, view, approve, reject, or discharge patients.
Discharge patients when treatment is complete.
Invoice Management:
Generate and download invoice PDFs, including charges for medicine, room, doctor, and other services.
Appointment Management:
View, book, approve, or reject appointments requested by patients.
Doctor Panel
Job Application:
Apply for a job at the hospital (requires admin approval to log in).
Patient Interaction:
View details of assigned patients (symptoms, name, mobile number).
Access the list of discharged patients.
Appointments:
View appointments booked by the admin.
Delete appointments after attending them.
Patient Panel
Account Management:
Create an account for hospital admission (requires admin approval to log in).
Doctor Details:
View assigned doctor information (specialization, mobile, address).
Appointments:
Book appointments (requires admin approval).
Check the status of booked appointments (pending/confirmed by admin).
Invoice:
View and download invoices after discharge by the admin.
How to Run the Project
Install Python

Install Python (version 3.7.6).
Ensure you check the "Add to Path" option during installation.
Install Dependencies
Open the terminal and run the following commands:

bash
Copy code
pip install django==3.0.5
pip install django-widget-tweaks
pip install xhtml2pdf
Download the Project

Download the project zip file and extract it.
Navigate to the project folder in the terminal.
Setup the Project
Execute the following commands:

bash
Copy code
py manage.py makemigrations
py manage.py migrate
py manage.py runserver
Access the Application

Open your browser and visit:
http://127.0.0.1:8000/
Changes Required for the Contact Us Page
Email Configuration in settings.py
Update the following variables with your email details:

python
Copy code
EMAIL_HOST_USER = 'youremail@gmail.com'
EMAIL_HOST_PASSWORD = 'your email password'
EMAIL_RECEIVING_USER = 'youremail@gmail.com'
Enable Less Secure App Access

Log in to your Gmail account.
Enable "Less Secure Apps" access by visiting:
Google Less Secure Apps
Drawbacks and Suggested Improvements
Admin Signup:

Currently, anyone can register as an admin without approval.
Suggested Fix: Disable admin signup and implement superuser creation logic.
Doctor Requirement:

At least one doctor must be added to the system before admitting patients.
Password Updates:

Passwords must be updated manually on the doctor and patient update pages.
This project provides a foundational structure for hospital management and can be extended further based on requirements.
