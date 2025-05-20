# Frontend Mentor - Four card feature section solution

This is a solution to the [Four card feature section challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/four-card-feature-section-weK1eFYK). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

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

## Overview

### The challenge

Users should be able to:

- View the optimal layout for the site depending on their device's screen size

### Screenshot

![](![alt text](image.png))


### Links

- Solution URL: (https://github.com/korcakSEA/four-card-feature-section.git)
- Live Site URL: (https://korcaksea.github.io/four-card-feature-section/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid
- Mobile-first workflow


### What I learned

Major learning for this project is the usage of grid-template-areas property.

Beside mobile first approach also helped me to design the page. All necessary properties are applied to elements at mobile first approach. And other properties (media query, grid-template-areas, :nth-child() ) applied when it is needed.

```
@media(min-width:900px){

    .grid-container{

        display: grid;

        grid-template-columns: repeat(3,1fr);

        /* grid-template-areas: arranging how cards to be laid out on page.
          Could be thought as blueprint of layout
        */
        grid-template-areas: 
         ".   two   ."
         "one two   four"
         "one three four"
         ".   three .";
    }

    /* If card are defined outside of media query, they are overlapped  */

    .card:nth-child(1){
    grid-area: one;
    }

    .card:nth-child(2){
        grid-area: two;
    }

    .card:nth-child(3){
        grid-area: three;
    }

    .card:nth-child(4){
        grid-area: four;
    }

}
```
### Continued development
Grid layout is a powerful property in CSS and I will continue using on in complex layout projects.

### Useful resources

- [Example resource 2](https://www.youtube.com/watch?v=JFbxl_VmIx0) - This helped me to understand how grid-template-areas works.


## Author

- Frontend Mentor - [@korcakSEA](https://www.frontendmentor.io/profile/korcakSEA)



