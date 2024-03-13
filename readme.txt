Udemy Course Content Downloader

Introduction:

This script is designed to download Udemy course contents and video URLs, divide sections, and save them in a .docx file.
Please note that you may not be able to download certain courses.

System Requirements:

Python 3
python-docx library 
SeleniumBase
chrome browser

install Requirements:

Open a PowerShell and run the following commands:
 ```bash
 pip3 install seleniumbase
 pip install python-docx

or you may need to install like this
C:\Python311\python.exe -m pip install seleniumbase
C:\Python311\python.exe -m pip install python-docx


Usage Instructions:

Enter your Udemy account credentials and the output folder path in the config file.
The config file is located inside the "scripts" folder.

Open the command prompt and run the following command:
python scripts\UdemyCourseContents.py <CourseUrl> <DestFolder>

EXplanation of Parameters:

<CourseUrl>: The path to the folder containing your Sinhala Unicode text files.
<DestFolder> (Optional): The path where you want the output file to be saved. If not provided, the "output" folder will be created within the config output folder path.

Example Usage:

cd C:\tmp\Avishka\UdemyCourseContents
C:\Python311\python scripts\UdemyCourseContents.py https://www.udemy.com/course/pythonforbeginnersintro/ output1

If you want to run without chrome background, add the headless argument:
C:\Python311\python scripts\UdemyCourseContents.py https://www.udemy.com/course/pythonforbeginnersintro/ output1 --headless

Note:
If you want to change the output format, especially the .docx margins,
rename your template to "00-template.docx" and place it inside the "scripts" folder.
