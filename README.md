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

![](solution.jpg)


### Links

- Live Site URL: [Add live site URL here]()

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox

### What I learned

1. How to put a div containing text and one containing an image side by side.

2. How to add color to an image:
```css
.flex-container-image {
    border-radius: 0px 10px 10px 0px;
    background: url(images/image-header-desktop.jpg);
    position: relative;
    overflow: hidden;
    height: 60%;
    width: 40%;
}

.flex-container-image-overlay {
    position: absolute;
    top: 0;
    left: 0;
    height:100%;
    width: 100%;
    background: rgba(170, 92, 219, 0.546); /* The color of the image is not accurate yet */
}
```

3. How to position text stacked on top of each other. This was the hardest part of the project for me for some reason. The text at the very bottom of the paragrpah is suppossed to be stacked like a column and then evenly spaced:
```html
<!-- Text below body-->
          <div class = "content-lower-body">
            <div>
              <h3>10k+</h3>
              <p>Companies</p>
            </div>
            <div>
              <h3>314</h3>
              <p>Templates</p>
            </div>
            <div>
              <h3>12M+</h3>
              <p>Queries</p>
            </div>
          </div>
      </div>
```
```css
.content-lower-body {
    display: flex;
}

.content-lower-body h3{
    font-size: 1em;
    line-height: 0.5;
    font-weight: 700;
    color: hsl(0, 0%, 100%);
    padding-left: 60px;
    padding-top: 20px;
}

.content-lower-body p{
    font-family: 'Inter';
    font-size: 0.8em;
    font-weight: 400;
    line-height: 0.5;
    color: hsla(0, 0%, 100%, 0.6);
    padding-left: 60px;

}
```
4. How to add rounded broders to only part of a div. I had no idea you could do that!:
```css
.flex-container-content {
    border-radius: 10px 0px 0px 10px;
    height: 60%;
    width: 40%;
    background-color: hsl(244, 38%, 16%);
}
```


If you want more help with writing markdown, we'd recommend checking out [The Markdown Guide](https://www.markdownguide.org/) to learn more.

### Continued development

1. Adding color to an image. I still need to find out how to add text to an image properly. There were many solutions i found online especially on stack overflow. The best ones included the use of filter and the use of a div overlay. I am yet to get the hang of it but I will!
2. Positioning, positioning, positioning. God this has been my bane for so long. Whether it be flex, grid or floats its always been a hard concept to grasp.
3. Naming github commits
4. Naming css/html classes
5. Indsutry standards 
6. responsive design
7. Cleaner programming solutions. No more hacky solutions!

### Useful resources

I found a lot of useful solutions during my development of this project (most on stack lol) but unfortunately i didnt save them. I know they are still in my browser histiry but i cant look for them all. However i have now learned to be saving them for suture use.


## Author

- Frontend Mentor - [@shemjay](https://www.frontendmentor.io/profile/shemjay)
- Twitter - [@shemstack](https://www.twitter.com/shemstack)


## Acknowledgments

Thanks to 'My name is Macca' on The Programmers Hangout discord for helping me with the positioning of the paragraph text!

