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
  - [Continued development](#continued-development)
  - [Useful resources](#useful-resources)
- [Author](#author)
- [Acknowledgments](#acknowledgments)

## Overview

### The challenge

Users should be able to:

- View the optimal layout depending on their device's screen size
- See hover states for interactive elements

### Screenshot

![](./images/nft-screenshot.png)

### Links

- Solution URL: [https://github.com/Grill3dCheese/FEM-NFTCard](https://github.com/Grill3dCheese/FEM-NFTCard)
- Live Site URL: [https://grill3dcheese.github.io/FEM-NFTCard](https://grill3dcheese.github.io/FEM-NFTCard)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox

### What I learned

Wow! This one was a doozy! Remember a couple of takeaways from this project:

1. SVG icons also need to be accessible! Here is a site I found on how to do that: -[SVG Accessibility](https://www.smashingmagazine.com/2021/05/accessible-svg-patterns-comparison/)
2. Remember the way you are setting up HTML structure. On this project I had some issues due to structure and was unable to get CSS transition fade on eye SVG icon to fade away with opacity box. When adding transition property you would see the eye move across the picture to center itself.
3. Also remember padding/margin as card was initally bouncing on load/reload. Again, due to the transition property being added to an element that had other properties - one being the margin property. I was able to specify the transition for "opacity" which helped in this situation.

- Thank you to W3Schools for walking me through the opacity hover box effect -[Opacity with Box](https://www.w3schools.com/howto/tryit.asp?filename=tryhow_css_image_overlay_opacity)

```html
<svg role="img" width="48" height="48" xmlns="http://www.w3.org/2000/svg">
  <title>Eye icon</title>
</svg>
```

^ Using the role attribute and title element to assist with SVG accessibility.

```css
.nft-image img {
  opacity: 1;
  border-radius: 0.75rem;
  transition: opacity 0.5s ease;
  cursor: pointer;
}
```

^ Setting transition property to specifically target opacity

### Continued development

- Continue learning all about accessibility and how to implement best practicies into all of my projects!
- Also continue to remember how each element interacts and impacts one another, divs within divs, etc.

### Useful resources

Check out ### What I learned section for helpful links I used in this project! :)

## Author

- Website - [Keith McKenna](https://www.keithmckenna.com)
- Frontend Mentor - [@Grill3dCheese](https://www.frontendmentor.io/profile/Grill3dCheese)
- Twitter - [@keithmckenna](https://www.twitter.com/keithmckenna)

## Acknowledgments

Thank you to W3Schools and Carie Fisher for the assists!! 😎
