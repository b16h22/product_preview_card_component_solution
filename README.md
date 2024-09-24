# Frontend Mentor - Product preview card component solution

This is a solution to the [Product preview card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/product-preview-card-component-GO7UmttRfa). 

## Table of contents

- [Overview](#overview)
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
- See hover and focus states for interactive elements

### Screenshot

![](./screenshots/desktop_design.png)
![](./screenshots/active_states.png)
![](./screenshots/mobile_design.png)

### Links

- Solution URL: [Github repo](https://github.com/b16h22/product_preview_card_component_solution)
- Live Site URL: [Github pages](https://b16h22.github.io/product_preview_card_component_solution/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox

### What I learned

Using meda queries and breakpoints to create a responsive layout that worked on Desktop and Mobile screens was a major part ofthis challenge. This is how I did it.

```css
    .card {
      display: flex;
      flex-direction: row;
    }

    .coverimg_desktop {
      max-width: 50%;
    }

    .coverimg_mobile {
      display: none;
    }

    .content {
      max-width: 50%;
    }
```

```css
    @media screen and (max-width:768px) {

      .container {
        height: 100%;
      }

      .card {
        flex-direction: column;
        margin: 1.5em;
      }

      .coverimg_mobile {
        display: block;
        max-width: 100%;
      }

      .coverimg_desktop {
        display: none;
      }

      .content {
        max-width: 100%;
      }
      
    }
```

### Useful resources

- [CSS Flexbox](https://www.w3schools.com/css/css3_flexbox.asp) - This is a good article that helped me understand CSS Flexbox and it's capabilities.
- [CSS Media Query](https://www.w3schools.com/css/css_rwd_mediaqueries.asp) - This is a good article that helped me understand CSS Media Query and responsive layouts.

## Author

- Frontend Mentor - [@b16h22](https://www.frontendmentor.io/profile/b16h22)