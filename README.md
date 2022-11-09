Longhorns Learn Django Project

User Overview:

Longhorns Learn is an interactive web application where college students can create or join chat rooms relating to classes at the University of Texas at Austin. These chat rooms are intended for multiple students to study or discuss something related to a specific class. Students can filter available chat rooms by class, contents, and titles and join as many rooms as they like. The application provides an activity feed as well, updating the feed with the newest chats among all chat rooms to help highlight questions and answers relating to recent material. Each student has a profile where they can customize their display names, biographies, and profile picture. 



Creator Note:

Before jumping into my implementation process, I would like to emphasize the origin and purpose of this django project. The purpose of this project was for me to learn a wide scope of the Django framework on my own as I have not used this framework in my school work. Much of the implementation process in this project was taught by a Developer/Instructor, Dennis Ivy, in his 7 hour Django course on YouTube. The complexity of the frontend design in Longhorns Learn is thanks to a theme that I downloaded on this instructor's GitHub. I later edited much of the downloaded theme to fit my own vision of what Longhorns Learn should look like, yet it was mostly styling changes with a little bit of structural change. Other than the remains of the download theme, this project was developed myself through the teachings in the Django course.   

Technical Overview:

Longhorns Learn is a django-only application. There is no frontend framework at use, and the application's database is the django-provided SQLite3 database. Longhorns Learn also encapsulates an api developed using the Django Rest Framework. This project is not deployed as of now, but I intend to deploy it on Heroku in the near future. 

The implementation process of this project was based off of the theme I chose. I made sure to implement the backend in a way that would match the frontend components in the theme so I could easily merge the two once completing the backend. I first implemented all url routes and views, and then created the four data models utilized in this project: rooms, topics, messages, and users. Once making sure the backend was properly routing between views and that the database was correctly tracking all models, I installed and slowly connected each file in the theme with the backend. I then built out the website's API to learn Django's Rest Framework. Once the project's frontend and backend components were running smoothly, I went back through the theme and restyled it to fit a "University of Texas" look. 

Project Showcase:

Sign-In / Register Page-
A user can sign into an existing account using an email and password or create a new account. Each account creation requires a display name, a unique username, a unique email, and a password. A default profile picture will be assigned upon creation, and the account's biography will start blank. A user can change their profile picture and biography in the settings page after registering. 

Sign In
<br />
<img src="/git_images/website_signin.png" width="500">

Sign Up
<br />
<img src="/git_images/website_signup.png" width="500">

Home Page-
The home page features a list of classes, discussion rooms, and an activity feed. Each room displays a title, the host, a description, the number of users that have interacted with this room, the relevant class, and a creation time stamp. Users can filter which rooms are to be shown by either clicking on a class on the left, or by searching for keywords in the top search bar. The right side features the activity feed that shows the most recent messages among all rooms. The current user is displayed on the top right in the navigation bar. 

Home
<br />
<img src="/git_images/website_home.png" width="500">

Example of filtering by topic
<br />
<img src="/git_images/website_bytopic.png" width="500">

Example of filtering by search keyword
<br />
<img src="/git_images/website_search.png" width="500">

Home Page on Mobile Device (or in a very narrow browser)
<br />
<img src="/git_images/website_mobile.png" width="500">

Browsing by Class on Mobile Device (or in a very small browser)
<br />
<img src="/git_images/website_topics.png" width="500">

Activity Feed on Mobile Device (or in a very narrow browser)
<br />
<img src="/git_images/website_activity_feed.png" width="500">

Dropdown for Settings (edit user profile) and Logout
<br />
<img src="/git_images/website_dropdown.png" width="500">

Discussion Room Page-
A user can create a new discussion room from the home page. Upon creating a room, a user must provide the room name, related class, and a description. Each discussion room features a room title, chat box, a host (room creator), the users that have interacted with or "joined" the room, and a time stamp of when the room was created. The chat box, obviously, shows all chats within the room with each chat displaying its corresponding user and time stamp. Only the host can edit or delete a room (as shown in the top left of the room), and users can only delete messages of their own. 

Create Room
<br />
<img src="/git_images/website_create_room.png" width="500">

Room
<br />
<img src="/git_images/website_room.png" width="500">

Deleting a room (same page for deleting a message)
<br />
<img src="/git_images/website_delete_room.png" width="500">

Profile Page-
Each user has a profile page that showcases their display name, unique username, profile picture, biography, and rooms that they have participated in. The recent activities on the right reflect only the messages that this user has posted. Upon clicking edit profile, a user can upload a new profile picture as well as edit their display name, unique username, their email, and their biography. 

Profile
<br />
<img src="/git_images/website_profile.png" width="500">

Edit Profile
<br />
<img src="/git_images/website_update_user.png" width="500">

Website API-
The API of Longhorns Learn is extremely basic and was more for learning purposes than for any real use, as this website isn't even deployed yet. The API was developed using Django's Rest Framework, and provides data for all created rooms in the website. 

API Routes
<br />
<img src="/git_images/website_api.png" width="500">

API Room Access
<br />
<img src="/git_images/wbesite_api_rooms.png" width="500">

