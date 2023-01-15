# Frontend Mentor - Designo agency website solution

![Designo preview](./design/desktop-preview.jpg)

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Useful resources](#useful-resources)
- [Author](#author)

## Overview

### The challenge

Users should be able to:

- View the optimal layout for each page depending on their device's screen size
- See hover states for all interactive elements throughout the site
- Receive an error message when the contact form is submitted if:
  - The `Name`, `Email Address` or `Your Message` fields are empty should show "Can't be empty"
  - The `Email Address` is not formatted correctly should show "Please use a valid email address"
- **Bonus**: View actual locations on the locations page maps (we recommend [Leaflet JS](https://leafletjs.com/) for this)

### Links

- [Visit site](https://huddle-alternating.vercel.app/)

## My process

### Built with

- Semantic HTML5 markup
- Flexbox
- Mobile-first workflow
- [Sass](https://sass-lang.com/) - CSS preprocessor

### What I learned

Took the chance on this simple page to try out Sass for the first time. I found the ability to modularize your stylesheets especially useful and the possibility to create utility classes with ease:

```scss
@mixin row {
  display: flex;
  flex-direction: row;
}

@mixin flexRow($row) {
  @if $row {
    @include row();
  } @else {
    @include column();
  }
}

@mixin flexContent($align: stretch, $justify: flex-start) {
  align-items: $align;
  justify-content: $justify;
}
```

### Useful resources

- [Practical way to organize your Sass files](https://medium.com/@brunofrontend/practical-way-to-organize-your-sass-files-98c27a2623a2) - This article helped me figure out how to organize my project.

## Author

- Frontend Mentor - [@hamilton-i7](https://www.frontendmentor.io/profile/hamilton-i7)
- Twitter - [@hamilton_i7](https://twitter.com/hamilton_i7)
