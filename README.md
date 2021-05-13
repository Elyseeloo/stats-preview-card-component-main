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
- [Author](#author)
- [Acknowledgments](#acknowledgments)


## Overview

### The challenge

Users should be able to:

- View the optimal layout depending on their device's screen size

### Screenshot

![](images/screenshot.png)


### Links

- Solution URL: [Add solution URL here](https://your-solution-url.com)
- Live Site URL: [Add live site URL here](https://your-live-site-url.com)

## My process

### Built with

- Semantic HTML5
- CSS3
- Flexbox
- Bootstrap

### What I learned

This was a fun challenge, and it was actually my first time using CSS Flexbox. I spent the initial attempt trying to solely use the Bootstrap columns but found it much more practical to simply apply the Flexbox properties instead. This also included a chance to play around with the flex-direction and reverse properties, which was especially useful when trying to rearrange the image from being on the left of the text to being on the top in mobile-view. I could not find a way to get this same result with Bootstrap alone.

I also had a chance to practice the media display property. I settled on 990px as the max-width for mobile because that was around the size _just before_ things started going wonky on my 15" laptop.

What was the hardest part of this challenge for me, was getting the purple color overlay on the image. This undoubtedly took me the longest amount of time to finish, but the result was well worth it. I first tackled the issue by creating an overlay div for the purple color. And this worked well enough in desktop view, but once switching over to mobile the div didn't align properly with the image. This was because the overlay was a child of the card element and not of the image. It wasn't until I made a separate class for the header tag the overlay was in and changed its position to relative (thus making it the parent of the overlay) that the overlay started to work properly.

Codes I'm Proud Of:

```html
<header class="col-lg-6 img-parent">
  <img src="images/image-header-desktop.jpg" class= "card-image" alt="work-friends-laughing">
    <div class="overlay">
</header>
```

```css
.card-image{
  height: 100%;
  width: 100%;
  border-top-right-radius:10px;
  border-bottom-right-radius:10px;
}
.img-parent{
  position: relative;
}
.overlay{
  height: 100%;
  width: 100%;
  background-color: hsl(277, 64%, 61%);
  position: absolute;
  top: 0;
  border-top-right-radius:10px;
  border-bottom-right-radius:10px;
  mix-blend-mode: multiply;
}
```

### Continued development

Some concepts I want to continue developing in are remembering to use Semantic HTML. For example, using tags such as ``<headers>``, ``<articles>``, ``<sections>``, and ``<asides>`` instead of mostly non-semantic markup like ``divs``. Also, even though I am familiar with Bootstrap and many of the design elements its capable of, I want to expand my working knowledge of pure CSS and only use Bootstrap when I need to override some of the unnecessary CSS that it applies to my page.

Another aspect I want to improve upon is making my code look professional, dry, and concise.

## Author

- LinkedIn - [Elyse Chambers](https://www.linkedin.com/in/elyse-chambers-698310164/)
- Frontend Mentor - [@Elyseeloo](https://www.frontendmentor.io/profile/Elyseeloo)

## Acknowledgments

Two very big helps to me in completing this project are Chamu and Silver Graph from the Slack Community.
