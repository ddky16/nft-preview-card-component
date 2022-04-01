# Frontend Mentor - NFT preview card component solution

This is a solution to the [NFT preview card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/nft-preview-card-component-SbdUL_w0U). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

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

- View the optimal layout depending on their device's screen size
- See hover states for interactive elements

### Screenshot

![Desktop View](/NFT%20Snapshot%20desktop%20view.png)
![Mobile View](/NFT%20Snapshot%20mobile%20view.png)

### Links

- Solution URL: [Solution URL here](https://github.com/ddky16/nft-preview-card-component)
- Live Site URL: [Live site URL here](https://glittering-bubblegum-59c467.netlify.app/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- Responsive website

### What I learned

```html
<!-- Learning new svg element semantic on HTML -->
<svg width="11" height="18" xmlns="http://www.w3.org/2000/svg">
  <path
    d="M11 10.216 5.5 18 0 10.216l5.5 3.263 5.5-3.262ZM5.5 0l5.496 9.169L5.5 12.43 0 9.17 5.5 0Z"
    fill="#00FFF8"
  />
</svg>
```

```css
/* Learning about position on element layout display */
#hero {
  position: relative;
  border-radius: 1rem;
  overflow: hidden;
}

/* Using opacity to animate the hover effect on the image element */
#hero img {
  opacity: 1;
  display: block;
  width: 100%;
  transition: 0.8s ease-out;
  object-fit: cover;
}

/* Learning positioning the element who have the position properties absolute. Working with top, left and transform translate to center the view svg image */
#hero svg {
  transition: 0.3s ease-out;
  opacity: 0;
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  text-align: center;
}

#hero:hover {
  cursor: pointer;
  background-color: var(--color-cyan);
}

#hero:hover img {
  opacity: 0.4;
}

#hero:hover svg {
  opacity: 1;
}
```

### Useful resources

- [Example resource 1](https://www.w3schools.com/howto/howto_css_image_overlay.asp) - This helped me for using animation to make overlay image in CSS, so whenever user hover the image it will make image overlay so we can push another or pop up new element with new opacity so the image opacity decreased.

## Author

- Frontend Mentor - [@ddky16](https://www.frontendmentor.io/profile/ddky16)
- Twitter - [@code_ddky](https://twitter.com/code_ddky)
