---
layout: post
title:      "React/Redux Final Project "
date:       2017-12-20 13:31:21 -0500
permalink:  react_redux_final_project
---


Please checkout my source code with the links below.

[](http://github.com/samsonyuwono/rec-league-app/tree/master/rec-league-api)
[](http://github.com/samsonyuwono/rec-league-app/tree/master/rec-league-client)

Due to my obsession with NBA basketball, my original plan for my final project was to create an NBA team search engine that would display a team's current roster and statistics. Unfortunately, due to the cost of acquiring an api from various sources, I had to change my plan.

For my final project,  I decided to create a rec league app that uses CRUD. My app allows a user to easily see all teams and team rosters within their league. In addition, a user can add teams to the database and assign players to teams.

One of the biggest challenges when building this project was building a team show page that would display a team's roster. In order to accomplish this task, I used my existing team and player actions that I already had. I then used those actions in componentDidMount().

<blockquote class="imgur-embed-pub" lang="en" data-id="a/GBQB7"><a href="//imgur.com/GBQB7"></a></blockquote><script async src="//s.imgur.com/min/embed.js" charset="utf-8"></script>

Within render(), I created a function called teamShow(). In teamShow() I used the team id  from of the current page and filtered it to match with the id found in the players object. Once this was accomplished I was able to return and display a team's roster which included player image and name.

<blockquote class="imgur-embed-pub" lang="en" data-id="a/kpNnl"><a href="//imgur.com/kpNnl"></a></blockquote><script async src="//s.imgur.com/min/embed.js" charset="utf-8"></script>

Once this was accomplished, I called teamShow() within the DOM.

My further plans for this project is incorporate authentication and team standings. 

