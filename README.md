# Frontend Mentor - Bento grid solution

This is a solution to the [Bento grid challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/bento-grid-RMydElrlOj). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
- [Author](#author)

## Overview

### The challenge

Users should be able to:

- View the optimal layout for the interface depending on their device's screen size

### Screenshot

<div style="display: flex; gap: 20px">
    <div>
        <img src="./public/screenshot-wide.png" alt="screenshot-wide" />
    </div>
    <div>
        <img src="./public/screenshot-phone.png" alt="screenshot-mobile" />
    </div>
</div>

### Links

- Solution URL: [Solution](https://www.frontendmentor.io/profile/mirfanwebdev)
- Live Site URL: [GitHub Page](https://mirfanwebdev.github.io/bento-grid/)

## My process

### Built with

- Semantic HTML5 markup
- Less.js
- Flexbox
- CSS Grid
- Mobile-first workflow

### What I learned

In this project, i learned to make grid layout within each media query. This oportunity also strengthen my fundamental css for image relative position. From this project i had manage to adjust different grid template without changing html.

This is how grid wrapper html looks like:

```html
<div class="wrapper">
  <div class="item title"></div>
  <div class="item section"></div>
  ...
</div>
```

This how grid template difference between media query:

```css
/* mobile screen */
.wrapper {
  grid-template-columns: 1fr;
}

@media screen and (min-width: 768px) {
  .wrapper {
    grid-template-columns: repeat(3, 1fr);
    grid-template-rows: repeat(4, 1fr);
  }
}

@media screen and (min-width: 1280px) {
    .wrapper {
        grid-template-columns: repeat(4, 1fr)
        grid-template-rows: repaeat(9, 1fr)
    }
}
```

## Author

- Website - [M. Irfan](https://mirfandev.tech)
- Frontend Mentor - [@mirfanwebdev](https://www.frontendmentor.io/profile/mirfanwebdev)
- Twitter - [@mirfanwebdev](https://https://twitter.com/mirfanwebdev)
