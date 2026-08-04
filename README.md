# Frontend Mentor - Stats preview card component solution

This is a solution to the [Stats preview card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/stats-preview-card-component-8JqbgoU62). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

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

**Note: Delete this note and update the table of contents based on what sections you keep.**

## Overview

### The challenge

Users should be able to:

- View the optimal layout depending on their device's screen size

### Screenshot

![Here's a screenshot of the stats component page from my view](/design/stats-component-screenshot.png)

### Links

- Solution URL: [Add solution URL here](https://your-solution-url.com)
- Live Site URL: [Add live site URL here](https://your-live-site-url.com)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- Mobile-first workflow

**Note: These are just examples. Delete this note and replace the list above with your own choices**

### What I learned

Nothing too crazy, although I did use the picture element for the first time. I guess it's used for the specific situation for when you have two images of the same but one's for desktop and one's for mobile. So I used the picture element to ensure responsiveness and so it wasn't using a background image or some weird stuff like that. And I used a technique that I saw in another solution of this to use mix-blend-mode to get the purple to show you through which I thought was genius

```html
<picture class="stats__image">
  <source
    media="(min-width: 600px)"
    srcset="./images/image-header-desktop.jpg"
  />
  <img
    src="./images/image-header-mobile.jpg"
    alt="A group of people working together in a modern office space"
  />
</picture>
```

```css
.stats__image {
  border-top-left-radius: 1rem;
  border-top-right-radius: 1rem;
  position: relative;
  background-color: var(--color-accent);
}

.stats__image > img {
  border-top-left-radius: 1rem;
  border-top-right-radius: 1rem;
  width: 100%;
  height: 100%;
  object-fit: cover;
  mix-blend-mode: multiply;
}
```

So as you can see the picture element is actually the purple background. Then the img element uses that mix-blend-mode to show through the purple background and with the picture element, it was genius!

### Continued development

Honestly for this project, the tablet responsiveness is terrible. I'm not proud of it but I did my best and at least the text is readable. The image is what I'm concerned with, as it's not visible at all. I was wondering if I should just keep the card vertical

**Note: Delete this note and the content within this section and replace with your own plans for continued development.**

### Useful resources

- [Josh Comeau's CSS Reset](https://www.joshwcomeau.com/css/custom-css-reset/) - I would modify some of the things in this reset, like the line-height line, but otherwise it's a great reset for getting things started when working on any project!

### AI Collaboration

I didn't actually use any AI. However I have a pro plan so I was able to hook up Codex into my workflow which will be useful for the future.

**Note: Delete this note and the content above if you didn't use AI, or replace with your own experience.**

## Author

- Website - [Noah D'Arcy](https://noahdarcy.dev)
- Frontend Mentor - [@darcynoa](https://www.frontendmentor.io/profile/darcynoa) (I need to change my username lol)
- Instagram - [@noahdarcy.dev](https://www.instagram.com/noahdarcy.dev)

**Note: Delete this note and add/remove/edit lines above based on what links you'd like to share.**
