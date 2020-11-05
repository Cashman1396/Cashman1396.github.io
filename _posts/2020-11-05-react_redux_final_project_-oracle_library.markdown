---
layout: post
title:      "React/Redux Final Project -Oracle Library"
date:       2020-11-05 06:58:27 +0000
permalink:  react_redux_final_project_-oracle_library
---


I can't believe that this is almost the end. My last project will be a culmination of the code, framework, terminology, and different programming languages I learned up to now. 

In my final project, I was tasked with creating a single-page web application (SPA) like before, but this time using the React frontend and Redux states to render out the different page from an HTML file as well as use Redux Thunk middleware to handle the asychronous fetch and dispatches to my reducers. 

My project called the Oracle Library is a upgraded idea from my Javascript and Rails project(Universal Catalog) with the past idea of my Sinatra project. Oracle Library is a library when users can hold different information that can store. When you need to keep track all the shows you have in a watchlist of shows but some are on Netflix,  others on Hulu, and some are just on some third party website. You can utilize this library just for that. If the user is a gamer like myself and needs to remember all the games that they have whether its physical or digital, they are able to input all that data into the library and edit or delete when they are done. Users are able to signup and login due to the authentication and session management from the frontend and backend. 

On the backend I use a ```sessions_controller``` to handle the authentication of the current user when they sign up or login. Then after they are login into the library and are the current user, the frontend handles the form data and current user that gets stored in the state of the redux store. 

In the beginning I was brainstorming some ideas asking friends and coworkers, looking for inspiration on what to create. When I had the idea for a record for tv shows then wanted to expand on that idea to get where we are now. I first created the database in the backend using ``` rails new   . . .  --api ``` to get everything started. Since this is what will be controlling the fetch requests, action creators, creating, updating, deleting, and dispatches that will be happening on the front end. I created controllers and seed that wil be initial data i could use as a test. 
```
 user = User.create([
    {username: "test",
    email: "test@email.com",
    password: "test"}])

user = User.create([
    {username: "Home",
    email: "home@email.com",
    password: "home"}])

test = User.first
test_game = test.video_games.create(
		
		game_name: "Pokemon Sword and Shield",
    
		game_genre: "Role-Playing Game",
    
		game_rating: "E for Everyone",
    
		game_platform: "Nintendo Switch",
    
		year_released: 2019,
    
		description: "Pokémon Sword[a] and Pokémon Shield[b] are 2019 role-playing video games developed by Game Freak and published by The Pokémon Company and Nintendo for the Nintendo Switch.",
    
		image_url: "https://upload.wikimedia.org/wikipedia/en/thumb/f/fa/Pok%C3%A9mon_Sword_and_Shield.jpg/440px-Pok%C3%A9mon_Sword_and_Shield.jpg")

    test_game = test.video_games.create(
        game_name: "Super Mario Sunshine",
        game_genre: "Platform",
        game_rating: "E for Everyone",
        game_platform: "Nintendo Gamecube, Nintendo Switch",
        year_released: 2002,
        description: "The game takes place on the tropical Isle Delfino, where Mario, Toadsworth, Princess Peach and five Toads are taking a vacation. A villain resembling Mario, known as Shadow Mario, vandalizes the island with graffiti and leaves Mario to be wrongfully convicted for the mess. Mario is ordered to clean up Isle Delfino, using a device called the Flash Liquidizer Ultra Dousing Device (F.L.U.D.D.), while saving Princess Peach from Shadow Mario.",
        image_url: "https://upload.wikimedia.org/wikipedia/en/7/78/Super_mario_sunshine.jpg"
        )
    
    test_game = test.video_games.create(
        game_name: "Crash Bandicoot 4:It's About Time",
        game_genre: "Platform",
        game_rating: "E 10+ for Everyone 10 and Up",
        game_platform: "Playstation 5, Playstation 4, Xbox Series X, Xbox One",
        year_released: 2020,
        description: "Main story levels focus on players controlling Crash and Coco, both of whom use identical movesets such as spinning and sliding, alongside new moves to the series such as wall running. In these levels, the characters are aided further by special masks, each of which is rescued during the story and who offers their powers – each level features at least one such mask being available to help traverse obstacles during certain segments, appearing before the player enters and leaving when the segment is traversed. Each mask has a specific property that dictates how it can help players overcome obstacles – for example, phasing objects in and out of existence.[9] Alternate timeline levels focus on players controlling one of three other playable characters during these levels: Doctor Neo Cortex, Dingodile, and Tawna.",
        image_url: "https://upload.wikimedia.org/wikipedia/en/3/39/Crash_Bandicoot_4_Box_Art.jpeg")```
				
The seed just holds a small sample of games to give an idea of what it actually can do. 

After I was finish building out my backend API, I got into the frontend using ``` create-react-app``` to build out the initial framework. I setup Redux, Thunk, and Navigation that I knew I would need for the project. I create 5 different reducers files for Redux to utilize: ```loginReducer, newVideoGameReducer, videoGamesReducer, signupForm and currentUser ```. Each of these reducers was helping React with a piece of the frontend. 

![](https://imgur.com/a/yoiuGaO)

# Hardest Part and Moving Forward
This project as the others was a lot ups and downs and very stressful at times to say the least. There were times, I got no sleep because all I was doing was thinking about to how fix the errors I kept getting. I pushed myself and tried my best to create a working project that I could be proud of and wanted to see the very project I made, the Oracle Library, come to fruition. It is the culmination of the languages of everything that I have learned these past 10 months and I am proud to have made it too this point. I hope to contain my utilizing what I have learned at Flatiron for where my path takes me after I finish. Moving forward, I thought this project was hard but at the same time it was a refresher to past things I learned as well as the new concepts, terms, and framework I recently learned.

I hope you enjoyed 
