Eureka_Website_Automation_Testing_Case_6

Overview

This repository contains the Case_6 automation script. It is developed using Python and Selenium to automate Access_Typed_Free_To_Read book and book chapter search and download actions via searching on the Eureka website. The script was developed in PyCharm IDE.

Test Case Summary:

This positive test case verifies that a user can successfully access and download assigned Access_Typed_Free_To_Read books or Access_Typed_Free_To_Read book chapters from the Eureka Website. The user logs in with valid credentials and then searches for the Access Book or Book Chapter by entering the title/keyword in the Search field and clicking the search button. If the selected book is assigned by the admin, the user is able to download the permitted content, either specific chapters or the complete book. The system displays the relevant chapter or books, and the user clicks on the Download button to complete the download.

Folder Structure

<img width="541" height="345" alt="image" src="https://github.com/user-attachments/assets/192d393a-cea3-4e00-a011-e5cc2fe34943" />


.env File

Purpose:

To securely store login credentials and the base URL.

Install dotenv library:

pip install python-dotenv

Python Code to Load .env File:

import os
from dotenv import load_dotenv

Load .env file
load_dotenv(".env")

Variables
EMAIL = os.getenv("EMAIL")
PASSWORD = os.getenv("PASSWORD")
BASE_URL = os.getenv("BASE_URL")

.env File Content:

LOGIN CREDENTIALS
EMAIL=(Your Email)
PASSWORD=(Your Password)

SITE URL
BASE_URL=https://www.eurekaselect.com/

Creating Executable (.exe) File

Install PyInstaller:

pip install pyinstaller

Command to Create Executable:

pyinstaller --onefile --collect-all selenium Case_6.py
