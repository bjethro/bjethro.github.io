---
layout: project
type: project
image: images/cotton-square.png
title: Quiz Game
permalink: projects/QuizGame
# All dates must be YYYY-MM-DD format!
date: 2018-5-01
labels:
  - Object Oriented Programming
  - C++
  - QT
  - GitHub
summary: Final Group Project for EE 205 (Object Oriented Programming)
---


 Our final EE205 project involved working with a team of 4 individuals and using the skills learning in class and lab to create a game using object orientend programming and the use of graphic libraries to bring the game to life. My task for this project was to implement the game screen using SFML to make the game more interactive and feel like a game.

A snipet of our code of displaying our gamescreen:

 
std::cout << "Enter gamescreen running" << std::endl;
//Load Background picture and create texture object
sf::Texture texture;
if (!texture.loadFromFile("gamescreen.jpg"))
{   //error message
std::cout << "ERROR: Gamescreen Background Image Unable to Load" << std::endl;
}

sf::Font Cammron;
if (!Cammron.loadFromFile("fonts/Cammron.ttf"))
{
// error message
std::cout << "ERROR: Cammron Font Unable to Load" << std::endl;
}

// Set texture as a sprite
sf::Sprite background(texture);
    
<img class="ui small floated squared image" src="../images/gamescreen.jpg">

"gamescreen.jpg"



Source: <a href="https://github.com/agasbarro36/EE205"><i class="large github icon "></i>agasbarro36/EE205</a>

