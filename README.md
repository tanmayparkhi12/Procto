Procto- An Automatic Exam Proctoring tool for Online Exams
About Procto
Procto is an online proctoring tool that Professors can use to create exams that are Proctored using AI. They can also view the status of each student taking the exam in Real-Time. It is fast, easy to use, and incredibly convenient with a minimalistic UI! To create an exam, just register and log in to your account, click on the Create Exam button and enter details like Exam Name, Google Form Link, Start Date and Time and duration. Procto generates a unique exam code that you can distribute among the students. The students start the exam by logging in and entering the exam code while the exam is running. While they are taking the exam they are proctored using an AI-based system. By entering the exam code, the professor can see the status of all the students in real-time.

Tech Stack
Frontend- React.js, Redux, Material-UI, Materialise.css Backend- Node.js, Express.js, Passport.js, JWT Database- MongoDB Atlas, Mongoose Deep Learning Model- Tensorflow Implementation of CocoSSD Object Detection Model

About The Author
Hello! I am Tanmay Parkhi, Final Year BE IT student at Sinhgad Institute Of Technology and Science, Pune. I am very passionate about software development and problem-solving.

If you wish to run it on your machine,

Clone the Repository
Move to the Procto folder cd Procto
Run npm install
Move to client directory and run npm install again. cd client and npm install
Move back to parent directory cd ..
Run command npm run dev npm run dev This concurrently runs server and frontend. Give a few seconds for frontend to load on localhost:3000
As a Professor:
Open home page. It might take some time to load for the first time, will be faster from the next time.
Click on Register, CHECK are you an Instructor to create a professor account.
Login to your account.
Click on Create Exam Button. Fill out the form. In the Exam Link option you can enter any link like Google form, Microsoft Form etc on which you have created the quiz. It is advised to use Google Form.
Click on Generate Code button, it generates a code and shows it in the corresponding input field. Note it down. Click Create Exam Button to create the exam.
Once the exam is live, you can enter the exam code in the homepage and click the Check Logs Button to see the status of the students giving the exam in real time. To refresh the table just click Check Logs again.
As a Student
Open home page It might take some time to load for the first time, will be faster from the next time.
Click on Register, UNCHECK are you an Instructor to create a professor account.
Login to your account.
When the exam has started, enter the exam code provided by your professor and click the button to start the exam.
Make sure you are sitting in a WELL LIT Room. Do not try to cheat because your actions are being recorded!
List of Features
Automatic Proctoring Features:
Person Detection: If the student leaves the frame and does not return within a few seconds, this action gets recorded.
Multiple People Detection: If at any point during the exam more than one person is visible through the webcam, this action gets recorded. Faces need not be visible as its person detection not face detection.
Mobile Detection: If the student is detected using a mobile phone during the exam, this action gets recorded.
Prohibited Object Detection: If the student tries to use a prohibited object like a Book or Laptop it gets recorded.
Tab Change Detection: The tool counts the number of time student tried to change the tab or open some other application.
Prohibited Key Press Detection: The tool counts the number of times the student tries to press a prohibited key (Ctrl, Alt). This is to discourage copy-paste and sharing exam questions with others or using other shortcuts.
Right-Click Prevention: Right-clicking when the exam is going on is not possible.
Exam Restart: If due to network or any other issue the exam gets interrupted, it is possible to restart the exam within the running time (between start and end of the exam), but the time lost is not recovered.
Note- Since in the current iteration of the project I am using google form link from professor instead of making questions in the application itself, it is impossible to put key listeners and right click prevention in it since its a third party app and React prevents it due to security reasons. To test these features, please do ctrl press, alt press and right click on left side of screen only.

Professor Side Features:
Simple to use exam creation dialog box which automatically copies generated exam code to Clipboard.
Dynamic Student Logs Table with sort by name, email, etc functionality, Pagination, no of entries per page selector and buttons for going to next and previous pages.
Advanced Search functionality for logs table. Can search by a part of name, email etc with search results getting updated as you type. It also allows you to sort in ascending or descending order based on each column by clicking on column header.
