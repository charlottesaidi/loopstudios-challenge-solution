# Frontend Mentor - Sunnyside agency landing page solution

Solution to the [Loopstudios Landing Page challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/loopstudios-landing-page-N88J5Onjw). 

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Useful resources](#useful-resources)
- [Author](#author)

## Overview

### The challenge

Users should be able to:

- View the optimal layout for the site depending on their device's screen size
- See hover states for all interactive elements on the page  

### Screenshot

![](./screenshot.png)

### Links

- [Live Site]()  

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- [JQuery](https://code.jquery.com/) - JS library  

### What I learned

Animating underlines that progressively widen when hovering on links:  

```html
<ul>
  <li><a href="#">About</a></li>
  <li><a href="#">...</a></li>
  ...
</ul>
```

```css
li a {display: block; position: relative}
li a::after {content: ''; position: absolute; bottom: -15px; left: 0; right: 0; width: 28px; margin: 0 auto; height: 3px; background-color: hsl(0, 0%, 100%); opacity: 0; transition: opacity 300ms, transform 300ms;}
li a:hover::after, header .menu_logo nav ul li a:focus::after {opacity: 1; transform: translate3d(0, 0.2em, 0);}
li a::after {opacity: 1; transform: scale(0); transform-origin: center;}
li a:hover::after, header .menu_logo nav ul li a:focus::after {transform: scale(1);}
```

### Useful resources

- [Css Irl Info](https://css-irl.info/animating-underlines/) - Gave me the solution for animating underlines   

## Author

- Frontend Mentor - [@charlottesaidi](https://www.frontendmentor.io/profile/charlottesaidi)
