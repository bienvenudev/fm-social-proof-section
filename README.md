# Frontend Mentor - Social proof section solution

This is a solution to the [Social proof section challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/social-proof-section-6e0qTv_bA). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

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

## Overview

### The challenge

Users should be able to:

- View the optimal layout for the section depending on their device's screen size

### Screenshot

![mobile demo](https://github.com/jwben1/fm-social-proof-section/assets/132217074/75023e10-e334-436c-a35c-0d7a150cbac5)
![desktop demo](https://github.com/jwben1/fm-social-proof-section/assets/132217074/736945d3-5aff-4487-82be-1a29948d724e)

### Links

- [Solution URL](https://www.frontendmentor.io/solutions/social-proof-section-using-css-grid-Sa7aVPoTb0)
- [Live Site URL](https://bienvenudev.github.io/fm-social-proof-section/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid
- Mobile-first workflow

### What I learned

- Fix accessibility issues that comes with emojis by adding semantic text to screen readers 
```html
<footer> 
Made with 
    <span aria-hidden="true">❤️</span>
    <span class="sr-only">love</span>
</footer>
```

- The :nth-of-type() is a valuable tool for certain styling needs, especially when dealing with sequential elements. However, for complex or dynamic styling requirements, or when clarity and specificity are priorities, using modifier classes can be a more effective approach.

```html
<div class="rating rating1"></div>
<div class="rating rating2"></div>
```

```css
.testimonial-intro :nth-child(1) {
  font-weight: var(--fw-bold);
}
.testimonial-intro :nth-child(2) {
  color: var(--clr-soft-pink);
}
```

- Using two images as a background image and positioning them, and also the using max to select the lowest the size can be.

```css
body {
  background-image: url(/images/bg-pattern-top-desktop.svg),
    url(/images/bg-pattern-bottom-desktop.svg);
  background-position: top left, bottom right;
  background-size: max(50%, 370px), max(50%, 370px);
}
```

### Continued development

- Using CSS Grid Columns and achieve the desired layout.

### Useful resources

- [Kevin Powell's Walkthrough](https://www.youtube.com/watch?v=K27WULzr2P8)

## Author

- [Frontend Mentor Profile](https://www.frontendmentor.io/profile/jwben1)
- [Linkedin](https://www.linkedin.com/in/bienvenu-cyuzuzo/)

## Acknowledgments

I had inspiration from Kevin Powell's solution and also feedback from the FEM Community.
