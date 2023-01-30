# Frontend Mentor - Fylo data storage component solution

This is a solution to the [Fylo data storage component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/fylo-data-storage-component-1dZPRbV5n). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
- [Author](#author)

**Note: Delete this note and update the table of contents based on what sections you keep.**

## Overview

### The challenge

Users should be able to:

- View the optimal layout for the site depending on their device's screen size

### Screenshot

Desktop 
![](./screenshots/Fylo%20Desktop.png)

Mobile  
![](./screenshots/Fylo%20Mobile.png)

### Links

- Solution URL: [Frontend Mentor](https://www.frontendmentor.io/solutions/responsive-fylo-data-storage-component-1GE0mxS-oe)
- Live Site URL: [GitHub](https://github.com/nicoams/fylo-data-storage)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- [Sass](sass-lang.com) - CSS Preprocessor

### What I learned

On this one I used ``::before`` and ``::after`` to make the progress bar and the white marker as it shows on the code below:

```
    .progress-bar{
        height: 1rem;
        width: 100%;
        background-color: $neutral-VeryDarkBlue;
        margin: 1rem 0 0.5rem 0;
        padding: 0.2rem;
        border-radius: 0.7rem;
        display: flex;

        &::before{
            content: "";
            height: 100%;
            width: 81%;
            background: $primary-Gradient;
            border-radius: 0.7rem;
        }

        &::after{
            content: "";
            height: 75%;
            width: 1.5%;
            background: white;
            position: relative;
            top: 4%;
            left: -1.7%;
            border-radius: 5rem;
        }
```

![](./screenshots/progress%20bar.png)

I also used ``position: relative`` to move it around. It was not what I wanted, since it is not that responsive. But I did not know a better alternative.

### Continued development

One of the biggest problems I faced on this project was keeping some things responsive, such as the pseudo-elements. I discovered they do not work well as they way I coded, but I do not know any other way for now, so I intend to improve that.

## Author

- GitHub - [Nicholas Albuquerque](https://github.com/nicoams)
- Frontend Mentor - [@nicoams](https://www.frontendmentor.io/profile/nicoams)