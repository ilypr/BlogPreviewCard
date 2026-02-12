# Responsive blog-preview-card solution

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshots)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Useful resources](#useful-resources)

## Overview

### The challenge

The main idea of the challenge was to build a blog-card webpage that would scale properly on both mobile and PC screens.

### Screenshots

Both PC and mobile versions of the webpage

### Links

- Solution URL: [Github](https://github.com/ilypr/BlogPreviewCard)
- Live Site URL: [Hosting](https://responsive-course-card.netlify.app/)

## My process

### Built with

- Semantic HTML5 (main, footer, sections)
- Flexbox
- Mobile-first workflow

### What I learned

In this project, I've tried my best at applying semantics in HTML code, as well as new CSS classes for the links (hover).
I learned how to connect a local font file to my CSS using @font-face; previously, I'd just use any font of my liking from the Internet. Other than that, I used the variable font weight in the @font-face class.
In the process of hosting the webpage, I've managed to resolve the problem with the wrong link paths, specifically, the images and the font-family.

As for the example, I had this line of code:

```css
@font-face {
  font-family: "local-font";
  src: url("/BlogPreviewCard/assets/fonts/Figtree-VariableFont_wght.ttf");
  font-weight: 500 800;
  font-style: normal;
}
```

The main problem with this code was that the font-style was working fine on my local machine, but when it came to the hosted webpage, it broke and wasn't showing any custom font whatsoever.
The fix for that problem was very simple; I just had to stop using absolute paths starting with a slash (/), and instead use relative paths.

### Useful resources

Generally, whenever I have troubles or issues with grasping information, I tend to go to w3schools website. This site has been a great help to me throughout my journey so far:

- This helped me with the understanding of the hover function: [CSS :hover Pseudo-class](https://www.w3schools.com/cssref/sel_hover.php)

- This article explained how to link and use a custom font: [CSS Custom Fonts](https://www.w3schools.com/css/css3_fonts.asp)
