---
layout: project
type: project
image: images/BoujeeFoodie.png
title: BoujeeFoodie
permalink: projects/BoujeeFoodie
# All dates must be YYYY-MM-DD format!
date: 2018-05-01
labels:
  - React
  - Meteor
  - ESlint
  - Meteor
summary: Final Group Project for ICS 314 (Software Engineering I)
---

Our final ICS 314 project was about creating a website from a template and implementing our knowledge and skills that we learned as software engineers in Professor Johnson's ICS class. We learned how to further advanced our knowledge on making a website, from front-end programming and back-end programming. It was a month long project that was separated in to 3 milestones in order for us to create the website from bottom up. In each milestones, I had variety of task. From implementing search bars to admin functionality.

Our final EE205 project involved working with a team of four individuals and using the skills learning in class and lab to create a game using object oriented programming and the use of graphic libraries to bring the game to life. My task for this project was to implement the game screen using SFML to make the game more interactive and feel like a game.

A snippet of our code of creating editing our search bar to display only the name and image of the restaurants related to the search. This also calls to view the restaurant whenever you select a restaurant that you desired:

    import PropTypes from 'prop-types';
    import React from 'react';
    import { Search } from 'semantic-ui-react';
    import { NavLink } from 'react-router-dom';
    import SearchBar from './SearchBar';
   
   
    const resultRenderer = ({ name, image, _id }) => {
     if (name)
       return (
           <Search.Result
               as={NavLink} activeClassName="" exact to={`/restaurantpage/${_id}`}
               title={name}
               image={image}
           />
       );
     };
   
    resultRenderer.propTypes = {
     name: PropTypes.string,
     description: PropTypes.string,
     image: PropTypes.string,
     _id: PropTypes.string,
    };
   
    const SearchBarCustom = () => (
       <SearchBar resultRenderer={resultRenderer}/>
    );
   
    export default SearchBarCustom;
  
 

<img class="ui floated squared image" src="../images/HomePage3.png">

Home Page of Boujeee Foodie

Source: <a href="https://boujeefoodie.github.io/"><i class="large github icon "></i>Boujee Foodie</a>


