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

**Note: Delete this note and update the table of contents based on what sections you keep.**

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

- HTML5
- CSS3
- Flexbox
- Bootstrap 5

### What I learned

This challenge was actually my first time using CSS Flexbox. I spent the initial attempt trying to solely use the Bootstrap columns but
found it much more practical to simply apply the Flexbox properties. This also included a chance to play around with the flex-direction and reverse properties as well, which was especially useful when trying to rearrange the image from being on the left of the text to being on the top in mobile-view. I could not find a way to have this same effect with Bootstrap alone.

I also had a chance to practice the media display property, which is always interesting. I settled on 990px as the max-width for mobile because that was around the size _just before_ things started going wonky on my 15" laptop.
Use this section to recap over some of your major learnings while working through this project. Writing these out and providing code samples of areas you want to highlight is a great way to reinforce your own knowledge.

Codes I'm Proud Of:

```html
<h1>Some HTML code I'm proud of</h1>

```

```css
@media (max-width: 990px){
  .card{
    text-align: center;
  }
  .card-image, .overlay{
    background-image: url(images/images-header-mobile.jpg);
    border-bottom-right-radius: 0;
    border-top-left-radius: 10px;
  }
  .flex-container{
    flex-direction: column-reverse;
  }
  .features-container{
    flex-direction: column;
    padding-bottom: 2%;
  }
}
```

### Continued development

Use this section to outline areas that you want to continue focusing on in future projects. These could be concepts you're still not completely comfortable with or techniques you found useful that you want to refine and perfect.

**Note: Delete this note and the content within this section and replace with your own plans for continued development.**

### Useful resources

- [Example resource 1](https://www.example.com) - This helped me for XYZ reason. I really liked this pattern and will use it going forward.
- [Example resource 2](https://www.example.com) - This is an amazing article which helped me finally understand XYZ. I'd recommend it to anyone still learning this concept.

**Note: Delete this note and replace the list above with resources that helped you during the challenge. These could come in handy for anyone viewing your solution or for yourself when you look back on this project in the future.**

## Author

- Website - [Add your name here](https://www.your-site.com)
- Frontend Mentor - [@yourusername](https://www.frontendmentor.io/profile/yourusername)
- Twitter - [@yourusername](https://www.twitter.com/yourusername)

## Acknowledgments

This is where you can give a hat tip to anyone who helped you out on this project. Perhaps you worked in a team or got some inspiration from someone else's solution. This is the perfect place to give them some credit.
