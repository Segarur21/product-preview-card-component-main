# Frontend Mentor - Product preview card component solution

This is a solution to the [Product preview card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/product-preview-card-component-GO7UmttRfa). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
  - [AI Collaboration](#ai-collaboration)
- [Author](#author)

## Overview

### The challenge

Users should be able to:

- View the optimal layout depending on their device's screen size
- See hover and focus states for interactive elements

### Screenshot

![Product preview card component](/images/screenshot.png)
### Links

- Solution URL: [https://github.com/Segarur21/product-preview-card-component-main](https://github.com/Segarur21/product-preview-card-component-main)
- Live Site URL: [https://segarur21.github.io/product-preview-card-component-main](https://segarur21.github.io/product-preview-card-component-main)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties 
- Flexbox 
- CSS Grid 
- Mobile-first workflow

### What I learned

1. **How `body` height affects Flexbox alignment:**
   I learned that the `body` element only takes up the height of its content by default (`height: auto`). To center a component both vertically and horizontally across the screen, setting `min-height: 100vh` on the `body` is necessary so Flexbox has actual vertical space to work with.

2. **Responsive images with HTML `<picture>`:**
   Using the semantic `<picture>` element allows swapping images cleanly between mobile and desktop using `media` queries without needing extra JavaScript:

```html
<picture>
  <source media="(min-width: 48rem)" srcset="./images/image-product-desktop.jpg" />
  <img class="product-image" src="./images/image-product-mobile.jpg" alt="Gabrielle Essence Eau De Parfum" />
</picture>
```

3. **Preventing text overflow in price tags:**
   Combining `display: flex`, `align-items: center`, and `flex-wrap: wrap` on price elements prevents numbers from overflowing outside the container on smaller screens.

### Continued development

- Continue practicing responsive layouts using CSS Grid and Flexbox.

### AI Collaboration

I worked with an AI collaborator (Gemini) as a thought partner and technical peer throughout this challenge.

- **Font rendering debugging**
- **Layout and centering**
- **Code optimization**

## Author

- Frontend Mentor - [@Sergio G.U.](https://www.frontendmentor.io/profile/Segarur21)