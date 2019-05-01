---
title: "SoftEng Group Project: Football Visualiser"
description: "A Software Engineering group project for visualising and analysing football games."
current: false
technology: Java, JavaFX, FXML
---

<img src="/assets/img/group-football-visualiser/FVlogoFinal.png" alt="app-logo" style="width:128px; display: inline-block; float: left; margin-right: 10px;"/>During the penultimate year of university, I was part of a software engineering group project in which we developed a working football visualiser application using real world match data. The data was gathered by sensors placed on every individual player as well as the ball itself. It was a year long project, the team consisted of 6 members including myself. The project was presented at the end of the year and won the best presentation prize.

The full product manual and description of features are available [HERE](/assets/docs/Product Manual.pdf).

At the start of the project we were given a large data set of a single football match, containing data of the ball and player's positions relative to the field over time. We took this data to build an entire application in Java using JavaFX for the GUI.

I was responsible for our GIT repository management, some individual views and controls of the application (as the application was developed in a MVC pattern), landing page, serialization of match data for saving and loading matches, design of the application, initial prototype design of the project for the pitching and most design assets including the logo and the presentation poster.

We worked in pairs and had frequent meetings. The project was planned beforehand following agile Kanban board (Trello in our case) style methods, including  requirements gathering, writing documentation, class diagrams, unit testing, user stories, time management with Gantt chart.

![app-screen](/assets/img/group-football-visualiser/app-screen.png)
![app-diagram](/assets/img/group-football-visualiser/app-diagram.png)
![app-heatmap](/assets/img/group-football-visualiser/app-heatmap.png)

The application includes:

+ A landing page with options to import a new match file or select already imported and saved matches
+ A functioning pitch screen with:
  + ability to watch the entire match play out
  + individual player and ball entities
  + seekbar/timeline to access any time location of the match
  + seekbar/timeline with added highlights which display interesting events during the match (goals, fighting for the ball)
  + score for both teams
  + statistical data of the match, including most goals by player etc.
  + individual statistics and diagrams for any player
  + heatmap for every player