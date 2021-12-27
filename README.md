# Frontend Mentor - Meet landing page solution

This is a solution to the [Meet landing page challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/meet-landing-page-rbTDS6OUR). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

![Design preview for Meet landing page](./images/preview.jpg)

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
  - [Useful resources](#useful-resources)
- [Author](#author)
<!-- - [Acknowledgments](#acknowledgments) -->

## Overview

### The challenge

Users should be able to:

- View the optimal layout depending on their device's screen size
- See hover states for interactive elements

### Links


- [Frontend Mentor - solution URL](https://www.frontendmentor.io/solutions/meet-landing-page-using-scss-bem-flexbox-5TTjolJB1)
- [Live Demo](https://stfnpczk.github.io/meet-landing-page/)

## My process

### Built with

- Semantic HTML5 markup
- BEM notation
- SCSS
- Flexbox
- CSS Grid
- Mobile-first workflow

### What I learned

- `flexbox and position absolute` : Looking for a way to move items outside of the flex container, I tried to apply `position: absolute` on the right and left image.  
This unfortunately only kind of worked, since the images are taken out of the flex flow.

```scss
 &__desktop-images {
      display: flex;
    }

    &__desktop-image--left {
      position: absolute;
      top: 169px;
      left: -32px;
    }

    &__desktop-image--right {
      position: absolute;
      top: 169px;
      right: -32px;
    }
```

- `grid minmax()` : This function helps to set a minimum (maximum) to which an grid item can shrink (grow).

```scss
.gallery {
    display: grid;
    grid-template-columns: repeat(2, minmax(0, 225px));
}
```

- `background-image and linear-gradient()` : This function can be used to set an image and background color at the same time. 
```scss
.footer {
  background-image: linear-gradient($teal, $teal),
  url("../assets/mobile/image-footer.jpg");
}
```



### Continued development

- I will look into alternatives to move items outside of a container without breaking up the flex flow.

### Useful resources



- [Flexbox and absolute positioning --> CSS-Tricks ](https://css-tricks.com/flexbox-and-absolute-positioning/) 
- [ minmax() --> MDN docs](hhttps://developer.mozilla.org/en-US/docs/Web/CSS/minmax()) 
- [Background-image overlayed with background-color in footer --> Stack Overflow question](https://stackoverflow.com/questions/34173169/background-image-overlayed-with-background-color-in-footer)

## Author

- Frontend Mentor - [@stfnpczk](https://www.frontendmentor.io/profile/stfnpczk)

<!-- - Website - [Add your name here](https://www.your-site.com) -->
<!-- - Twitter - [@yourusername](https://www.twitter.com/yourusername) -->

<!-- ## Acknowledgments
**ADD TEXT**
This is where you can give a hat tip to anyone who helped you out on this project. Perhaps you worked in a team or got some inspiration from someone else's solution. This is the perfect place to give them some credit. -->
