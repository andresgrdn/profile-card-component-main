# Frontend Mentor - Profile card component solution

This is a solution to the [Profile card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/profile-card-component-cfArpWshJ). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
  - [Useful resources](#useful-resources)
- [Author](#author)
- [Acknowledgments](#acknowledgments)

**Note: Delete this note and update the table of contents based on what sections you keep.**

## Overview

### The challenge

- Build out the project to the designs provided

### Screenshot

![](./project-card-profile_.png)

### Links

- Solution URL: [github.com/andresgrdn/project-code](https://andresgrdn.github.io/)
- Live Site URL: [andresgrdn.github.io/project-page](https://github.com/andresgrdn/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid
- Mobile-first workflow

### What I learned

#### -> How background positioning an image

I learn to position many images using the background property, changing on my way of thinking about the position with the background-position.

Instead of thinking with percentages for positioning the circle with respect of the origin of the image, I used the position property, thinking how much space I need from the edge of the page to the end of the image.

```css
body {
  /* some code... */

  background-image:
    url("../images/bg-pattern-top.svg"),
    url("../images/bg-pattern-bottom.svg");

  background-position:
    calc(100% - 55vw) calc(100% - 45vh),
    55vw 45vh;

  background-size:
    900px,
    900px;

  /* some code... */
}
```

#### -> That I need to think about the grid model items sizing

There are some things about sizing with the grid model that I need to deep dive. I had an issue with the grid item because no matter what configuration I use for the box container, I can't achieve to make it fit to the content. Because of the grid model That I used for center the card container.

```css
body {
  display: grid;
  place-content: center;

  /* Some code... */
}
.card {
  /* Some code... */
  margin: 0;
  width: 25vw;
  min-width: 337px;
  height: auto;
  min-height: 355px;

  /* Some code... */
  overflow: auto;
}
```

### Continued development

I had some issues with the units beheivour when I use it with the background property.

### Useful resources

- [Background docs on the MDN website](https://developer.mozilla.org/en-US/docs/Web/CSS/background) - This helped me for to understand the default values that the background property has and what I need to overwrite.
- [CSSWG page on backgrounds](https://drafts.csswg.org/css-backgrounds/#the-background) - This page help me to understand the order of the values to modify the background image.

## Author

- Website - [Andres Gordon](https://andresgrdn.github.io)
- Frontend Mentor - [@andresgrdn](https://www.frontendmentor.io/profile/andresgrdn)
- Twitter - [@andresgrdn](https://www.twitter.com/andresgrdn)