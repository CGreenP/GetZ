# GetZ
A GUI To-Do List with Python and SQLite3.

## Introduction:
In this project, we'll create a feature-rich to-do list desktop application using Python libraries like tkinter, tkcalendar, sqlite3, APScheduler, random, time, and datetime. The app allows adding, deleting, and sorting tasks. Tasks with date and time reminders can be added and managed efficiently.

## Prerequisite:
1. Download and Install Python 3 (64 bit)
Download Link: https://www.python.org/downloads/windows/
2. Open CMD/PowerShell and type the following commands to install the required libraries to run the application.
* tkcalendar
```bash
pip install tkcalendar
```
* APScheduler
```bash
pip install APScheduler
```
3. After installing the required libraries, go to the src folder and double-click on the GetZ.py file  to run the application.

## ARCHITECTURE:
The project uses a database to save to entries in To-Do List and Tkinter for GUI. When we enter a task in To-Do List and select a date, the task is saved in database. When we enter the time, the task get updated. When we delete the task, it's get deleted from the database. The APScheduler checks if the current time and the time given in the database is equal or not. If they are equal, We will get a pop-up.

The entire project is done in generally two parts. They are – (a) GUI part And (b) Database part.

(a)	GUI Part: 

(i) At first we have created our main window(root) using tkinter module. Then we added all buttons, labels, listbox etc. in it using tkinter.

(ii)  Then we added a statusbar in the root window for loading the application using time module.

(iii)  Then we added a pop-up during adding task so that the user can add timer with the task to remind him about that particular task in that particular time. This pop-up has three buttons in it - a. Dateentry, b. Time and c. Exit. The dateentry button will accept date from user from a calendar in it. This calendar is created using tkcalendar. Next, the time button is there to accept time from user. And finally, the Exit button is there to exit from this pop-up. 

(iv) Next, we made another pop-up which will remind user about a task in the particular time which user chose. For this purpose we have used datetime and apscheduler module.

(b)	Database Part:

(i) When the user adds a task and don’t not set a reminder, the task is added. When the user adds a task and set a reminder, after selecting the date from the calendar, the task is added to the database with the default time 12 midnight. When the user selects the time, that task is updated. 

(ii) When the user deletes one task, that task is deleted from the database.

(iii) When the user deletes all the tasks, all the task is deleted from the database.

(iv) When the user sorts the list of task, all the tasks are fetched from the database and then they are sorted. After sorting the tasks, they are displayed.

## Sample Output:
![image](https://github.com/CGreenP/GetZ/assets/56307530/9937c5e1-8bd9-4ebd-b8d1-715f28ce27bd)

![image](https://github.com/CGreenP/GetZ/assets/56307530/fa7801a1-83ea-4028-94f8-de08f6e84da1)

![image](https://github.com/CGreenP/GetZ/assets/56307530/5059b91d-0875-4af4-991e-5bd394717c5b)

![image](https://github.com/CGreenP/GetZ/assets/56307530/4ff880a9-83c8-4cc5-81e6-3687e8fde4df)

![image](https://github.com/CGreenP/GetZ/assets/56307530/9485aef9-f708-4716-86b0-d09949421a87)

![image](https://github.com/CGreenP/GetZ/assets/56307530/aa7aff46-4845-4ec6-a25e-977dca71a7e8)

![image](https://github.com/CGreenP/GetZ/assets/56307530/20cb96c1-570f-4fe8-8a95-334b81652f15)

![image](https://github.com/CGreenP/GetZ/assets/56307530/87e869cf-1cf0-48c5-ad75-705ae2b5ace7)

![image](https://github.com/CGreenP/GetZ/assets/56307530/066a7225-a23a-4c68-82a7-0bfd0bb58962)

![image](https://github.com/CGreenP/GetZ/assets/56307530/524226df-8d54-4e67-a305-c134eb5ab1a4)

![image](https://github.com/CGreenP/GetZ/assets/56307530/7c0ae9f4-b035-4a59-82ed-c325b0093acb)

![image](https://github.com/CGreenP/GetZ/assets/56307530/7ed1d8e4-b4a2-4e3b-a7b7-539142248ed6)

![image](https://github.com/CGreenP/GetZ/assets/56307530/2bd0ed14-47f4-4d35-a67c-4caa884d2851)

![image](https://github.com/CGreenP/GetZ/assets/56307530/bda702f0-8aab-4f48-8faf-f9897cb3c81c)

![image](https://github.com/CGreenP/GetZ/assets/56307530/91c3f690-17d5-4d09-93c2-e8f060852577)
