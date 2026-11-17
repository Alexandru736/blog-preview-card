# Frontend Mentor - Blog preview card solution

This is a solution to the [Blog preview card challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/blog-preview-card-ckPaj01IcS). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

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
  - [AI Collaboration](#ai-collaboration)
- [Author](#author)

## Overview

### The challenge

Users should be able to:

- See hover and focus states for all interactive elements on the page

### Screenshot

![](./blog-preview-card.jpg)

### Links

- Solution URL: [GithubRepo](https://github.com/Alexandru736/blog-preview-card)
- Live Site URL: [LiveSite](https://blog-preview-card-alexandru.netlify.app/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox

### What I learned

During this challenge I was able to reinforce some knowledge about:

**CSS layout**

It's interesting to know that when the screen width or height are too short, you could use **padding** in the body, together with **max-width** and **width: 100%**, without even using media queries. 

Like here: 

```css
.card-wrapper {
    max-width: 384px;
    width: 100%;
}

body {
    padding: 1.5rem;
}
```

Another thing would be the clariying aspect between the **min-height** and **height**. There is a subtle difference when handling **short screens**. If you set the *height of the body* to 100vh, the body has exactly the height of the device. However, that was an issue when handling components that had a height bigger that the viewport height because the extra spilled card height would be distribute negatively and therefore you would have a bitten card. This is where I understood that it's very important to set the body to a *min-height: 100vh*. In this way, you would have the body at least as tall as the window and it could grow if the content needs more room. This would give you a scroll bar for you to scroll through taller components. 

One last thing would be about **align-self**. When I would use flexbox, I saw that the child items would stretch to the full available width to them. The "Learning" label needs to be a small label only. The `align-self: flex-start` helped me understand that this turns the label to use as much width as the content has, and not the full width.

### Continued development

Responsiveness feels very important to make your components flexible regardless of the screen resolution that you use. I want to master using it on multiple screen resolutions. 

### Useful resources

-  [Focus visible doc](https://developer.mozilla.org/en-US/docs/Web/CSS/Reference/Selectors/:focus-visible) - This helped me to understand more about focus-visible pseudo-class, used mostly for those who don't have a mouse and use Tab to access the clickable components.
- [Border doc](https://developer.mozilla.org/en-US/docs/Web/CSS/Reference/Properties/border) - This helped me understand how to add border lines around the edges of the `.card-wrapper` that don't have shadows.

### AI Collaboration

I used Cursor a lot for this challenge. I refrained from using it to build me boilerplate code. I'm at a stage where everything is a means to learn so I've been using AI to ask questions to evaluate current solutions. It feels so good to be able to understand things so easily and be able to apply them as well.

## Author

- Website - [BlogPreviewCardWebsite](https://blog-preview-card-alexandru.netlify.app/)
- Frontend Mentor - [Alexandru@](https://www.frontendmentor.io/profile/Alexandru736)
