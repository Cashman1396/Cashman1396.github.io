---
layout: post
title:      "Sinatra CMS Project - Video Game Database"
date:       2020-04-29 13:15:17 -0400
permalink:  sinatra_cms_project_-_video_game_database
---

This week I am finishing my Sinatra CMS project, and to keep with a theme I am doing a video game database. In this database, users can sign up using an email, username, and password this. After the user signs up or logins, the site will redirect them  to the home page where they can add video games to a database on the server that holds all the video games that they have entered into a form. The add games form consists of the Game Title, the Developer, the Publisher, and the Genre of the game. Once the user has entered any of these boxes, the site will redirect back to the homepage with the added game in their list. This is similar to how in the Fwitter lab, users can sign up or login and once they were logged in(thanks to the helper logged_in?) they could make and delete tweets. When the users are done, they can log out and it will send them back to the home page. I have also added in my old college project to show that the site can also be redirected to something outside of its scope just a little call back to the video game wikipedia I made back in college. 

When creating this project, I first thought out what I wanted to do, I made diagrams, looked through the learn videos, and asked people for some ideas. It then hit me that I could create a subsite to that wikipedia I made back in college, because more than often a lot of gamers play a ton of games and forget how many games they played or have. This site can help with that as well as giving them some information about that game. I thought it was a great idea to create and since it is similar to the some of the labs, I did it was a bit difficult to troubleshoot, but it was very easy to the understand the problems. 

In this project, we have 3 controllers: Application, User, and VideoGame. The application one controls the entire project like a supervisor, it looks for the current user, checks if they are logged in and searches for their session. Once the it has found those 3 pieces it hands it off to the User controller where this controller runs the sign up and log in. In here with the help of the has_secure_password in the models/user.rb, users can create secure passwords that will allow them to sign up/login into the site. The passwords are also checked through the usage of user.authenticate(params[:password]) line of code. Once the signup/login has be completed, the user controller will move the user to the VideoGame controller which runs the the forms of the site. In this part, the user has signed and been redirected to the videogame index page. This is where the site welcomes you and tells you that your list is empty so you should input a game. 

In the videogames/edit, users are given a form to input the information of any game. An example would be: Game Title: Pokemon, Developer: Game Freak, Publisher: Nintendo, Genre: Role-Playing Game(RPG). After they have finished that the inputted game would appear in your games list, congratulations the first game has inputted into the list. From there, users can click on the game, and it will give you the information that you have inputted from the videogames/edit. Users can now add a new game to their list, delete the game that is being shown, the edit game button does work, or logout. 

This project has shown me how to run a database using Sinatra , learn what the HTTP verbs do and how they work, as well as show the correlation between the Models, Views, and the Controllers cause its a MVC. 

```
https://github.com/Cashman1396/SinatraCMS-Project-
```
