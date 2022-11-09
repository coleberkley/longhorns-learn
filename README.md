Longhorns Learn Django Project

User Overview:

Longhorns Learn is an interactive web application where college students can create or join chat rooms relating to classes at the University of Texas at Austin. These chat rooms are intended for multiple students to study or discuss something related to a specific class. Students can filter available chat rooms by class, contents, and titles and join as many rooms as they like. The application provides an activity feed as well, updating the feed with the newest chats among all chat rooms to help highlight questions and answers relating to recent material. Each student has a profile where they can customize their display names, biographies, and profile picture. 



Creator Note:

Before jumping into my implementation process, I would like to emphasize the origin and purpose of this django project. The purpose of this project was for me to learn a wide scope of the Django framework on my own as I have not used this framework in my school work. Much of the implementation process in this project was taught by a Developer/Instructor, Dennis Ivy, in his 7 hour Django course on YouTube. The complexity of the frontend design in Longhorns Learn is thanks to a theme that I downloaded on this instructor's GitHub. I later edited much of the downloaded theme to fit my own vision of what Longhorns Learn should look like, yet it was mostly styling changes with a little bit of structural change. Other than the remains of the download theme, this project was developed myself through the teachings in the Django course.   

Technical Overview:

Longhorns Learn is a django-only application. There is no frontend framework at use, and the application's database is the django-provided SQLite3 database. Longhorns Learn also encapsulates an api developed using the Django Rest Framework. This project is not deployed as of now, but I intend to deploy it on Heroku in the near future. 

The implementation process of this project was based off of the theme I chose. I made sure to implement the backend in a way that would match the frontend components in the theme so I could easily merge the two once completing the backend. I first implemented all url routes and views, and then created the four data models utilized in this project: rooms, topics, messages, and users. Once making sure the backend was properly routing between views and that the database was correctly tracking all models, I installed and slowly connected each file in the theme with the backend. I then built out the website's API to learn Django's Rest Framework. Once the project's frontend and backend components were running smoothly, I went back through the theme and restyled it to fit a "University of Texas" look. 

Project Showcase:

<img src="/git_images/website_home.png" width="500">


This is a test:

<img src="/git_images/website_activity_feed.png" width="500">
