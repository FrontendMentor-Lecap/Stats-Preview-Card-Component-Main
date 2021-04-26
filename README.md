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
  - [Continued development](#continued-development)

**Note: Delete this note and update the table of contents based on what sections you keep.**

## Overview

### The challenge

Users should be able to:

- View the optimal layout depending on their device's screen size

### Screenshot

![](./images/screenshot.png)

### Links

- Solution URL: [https://github.com/FrontendMentor-Lecap/Stats-Preview-Card-Component-Main]
- Live Site URL: [https://frontendmentor-lecap.github.io/Stats-Preview-Card-Component-Main/]

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid
- Mobile-first workflow

### What I learned

I believe the most challenging part in this project was the image placement and color variation. I learned a lot of techniques that change the color of images including filters, layering and pseudo-elements.

In this case I used ::after in the parent element setting a background color of purple and an opacity of 0.6:

```css
.card__image::after {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background-color: purple;
  opacity: 0.6;
}
```

The image was placed as a child element, and the positioning was done by using

```css
#mobile-image {
  width: 100%;
  height: 100%;
  filter: grayscale(100%);
}
```

### Continued development

I want to continue playing with images (colors, positioning,filters, etc.). I also need to improve using flex-basis, growth and shrink in order to reduce the use of media queries. I would like to reduce the amount of code for individual components such as this one.
