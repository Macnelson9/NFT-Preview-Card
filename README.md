# NFT-Preview-Card
This is a solution to the [NFT preview card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/nft-preview-card-component-SbdUL_w0U). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
- [Author](#author)
- [Acknowledgments](#acknowledgments)

## Overview

This is a solution to the [NFT preview card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/nft-preview-card-component-SbdUL_w0U).
I am glad to be able to attempt this challenge, it took me more time than I had anticipated to solve this but I'm glad I got it done.

### The challenge

Users should be able to:

- View the optimal layout depending on their device's screen size
- See hover states for interactive elements

### Links

- Solution URL: [Add solution URL here](https://your-solution-url.com)
- Live Site URL: [Add live site URL here](https://your-live-site-url.com)

## My process

I started out first by taking a critical look at the design images where I figured what needed to be done. I figured that I'd need a div overlay for the hover active state on the image and to house the view icon but as at the time I began this project, I didn't know how to get it done. But I proceeded further to build the project and figure it out along the way. So, I built everything up until it was time to include the active state for the image and I got stuck. When I hover on the image, the overlay will appear behind the image and I just couldn't get it to come to the front even though I tried to use the z-index property lol. But after prompting ChatGPT, I got it figured out. Happy Coding!

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox

### What I learned

Phewwww, after spending 2 whole days on this project, I learnt how to add an overlay on an element when it is hovered on. And also, I learnt another media query selector.

To see how you can add code snippets, see below:

```html
<div class="image-container">
  <img src="./images/image-equilibrium.jpg" alt="Equilibrium" />

  <div class="overlay">
    <img src="./images/icon-view.svg" alt="view icon" />
  </div>
</div>
```

```css
image-container {
  position: relative;
  width: 100%;
  border-radius: 20px;
  overflow: hidden;
}

.image-container img {
  width: 100%;
  height: 100%;
  object-fit: contain;
  border-radius: 20px;
}

.image-container .overlay {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background: #00fff7ad;
  opacity: 0;
  transition: opacity 0.2s ease;
}

.overlay img {
  position: absolute;
  width: 15%;
  height: 15%;
  top: 120px;
  left: 115px;
}

/* this is the active state mechanism */
.image-container:hover .overlay {
  opacity: 1;
}

/* the media query selector */

@media (min-width: 601px) and (max-width: 1200px) {
  .container {
    width: 50%;
  }

  section.price img.clock {
    padding-left: 70px;
  }
}
```

## Author

- Frontend Mentor - [@macnelson9](https://www.frontendmentor.io/profile/Macnelson9)
- Twitter - [@macnelson92](https://www.x.com/macnelson92)
- LinkedIn - [@Uche Ofatu] (https://www.linkedin.com/in/uche-ofatu)

## Acknowledgments

Thanks to ChatGPT. Lol.

