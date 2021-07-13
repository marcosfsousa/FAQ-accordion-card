# Frontend Mentor - FAQ accordion card solution

This is a solution to the [FAQ accordion card challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/faq-accordion-card-XlyjD0Oam). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

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

- View the optimal layout for the component depending on their device's screen size
- See hover states for all interactive elements on the page
- Hide/Show the answer to a question when the question is clicked

### Screenshot

![Desktop](.\images\FAQ_accordion_desktop.png)
![Mobile](.\images\FAQ_accordion_mobile.png)


### Links

- Solution URL: [https://www.frontendmentor.io/challenges/faq-accordion-card-XlyjD0Oam/hub/faq-accordion-with-html-and-css-3XbZK2KsL]
- Live Site URL: [https://marcosfsousa.github.io/FAQ-accordion-card/]

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- Mobile-first workflow


### What I learned

Using pseudo-elements like :after and also using the trigger functionality of the general sibling combinator (~). 

 Here are some snippets to exemplify:
 
```css
.question_input:checked ~ .answer {
    display: block;
}

.question_input:checked ~ .question_label::after {
    transform: translateY(-50%) rotate(0.5turn);
}

.question_label::after {
    content: "";
    position: absolute;
    top: 50%;
    transform: translateY(-50%);
    right: 70px;
    width: 10px;
    height: 7px;
    background-image: url(images/icon-arrow-down.svg);
    background-size: contain;
    transition: transform 400ms;
```

### Continued development

Responsiveness
Image positioning

### Useful resources

- [dcode Youtube Channel] (https://www.youtube.com/watch?v=pzy_QStQaqA&t=1s) - This helped me for figuring out the accordion functionality using only CSS.

## Author

- Frontend Mentor - [@marcosfsousa](https://www.frontendmentor.io/profile/marcosfsousa)
- Github - [@marcosfsousa](https://github.com/marcosfsousa)

