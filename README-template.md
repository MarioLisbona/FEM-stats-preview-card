# Frontend Mentor - Stats preview card component solution

This is a solution to the [Stats preview card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/stats-preview-card-component-8JqbgoU62). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
- [Author](#author)


**Note: Delete this note and update the table of contents based on what sections you keep.**

## Overview

### The challenge

Users should be able to:

- View the optimal layout depending on their device's screen size

### Screenshot

![Fullsreen Desktop](./screenshots/fullscreen-desktop.png)
![Image Overlay Issue](./screenshots/image-overlay-issue.png)
![Mobile 1](./screenshots/mobile-1.png)
![Mobile 2](./screenshots/mobile-2.png)

### Links

- Solution URL: [Add solution URL here](https://github.com/MarioLisbona/FEM-stats-preview-card)
- Live Site URL: [Add live site URL here](https://mariolisbona.github.io/FEM-stats-preview-card/)

## My process

I created a main container div to hold the image container and information container. I set the max width's on both these containers for desktop. I then set the max-width: 100% for the image so it will fill the container as the container shrinks.

I set the elements into the information container, adding necessary padding between elements to make the container the same height as the image container. I sourrounded the word "insights" in a span element with a class 'accent' to change the color of that text.

I created a stats-container and had each number in its own div. I then created ::after elements for each number with its assosicated heading beneath the number.

I also created a ::after element to tint the image.

For mobile responsive, i changed the stylings of the info container to be center justified and adjusted the padding and border radius. I changed the main-container to flex:wrap with a dirction of column reverse so that the picture would be at the top of the page.

There is a slight overlap of the overlay on the image at the bottom. See screenshots. Its only a few pixels but i cant seem to get it to overlay exactly.

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox

### What I learned

I havnt used ::after element much and was struggling with the sizing of the color overlay. i was trying to use width: 100% and it was working. I figured out to set position: absolute inside the ::after element and poisiton: realtive on its parent.

## Author

- Frontend Mentor - [@MarioLisbona](https://www.frontendmentor.io/profile/MarioLisbona)

