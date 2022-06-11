# Drum Kit in JavaScript

Descripton: The Complete 2022 Web Development Bootcamp, Section 13: Advanced JavaScript and DOM Manipulation - Dr. Angela Yu

I will document my progress in this project through my commits and through the contents of this README file here on GitHub. 

## Table of contents

- [Overview](#overview)
  - [Screenshot](#screenshot)
  - [Link(s) to the Live Site](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
  - [Useful resource](#useful-resource)
- [Author](#author)
- [Acknowledgments](#acknowledgments)

## Overview

Again I was given completed HTML and CSS files, along with image and sound files.  My job was to put everything together, using Javascript, to 1. create clickable illustrated buttons that play particular sounds, and 2. create an option for using key presses to play the drum set. This was a very thorough and rewarding project!

### Screenshot

|    | 
|:--:|
| [![Image of Drum Kit on Various Devices Coming Soon](link-to-slides.png)]() |
| [Direct Link to the Drum Kit on AmIResponsive Website Comming Soon!]()|


### Links

- Live Site URL: [Play on CodePen!](https://codepen.io/faraja17/full/zYRmXLr)

## My process

As usual, I paused the video whenever it was recommended to do so. This project was much more challenging than the Dicee project, and I was not able to solve everything independently, but I learned A LOT, and I took my time to be sure I understood each concept before proceeding to the next step. 

There was a point when I became stuck for two hours and could not identify any bugs. I consulted the Q and A message boards and discovered that several classmates had had the same problem. For some reason that those classmates and I still have not figured out, `this.innerHTML` would not work. Some classmates figured out that using `this.textContent` worked, but then the strangest thing--changing back afterwards to `this.innerHTML` suddenly worked. I confirmed this to be true!

My final step will be to make the site responsive. I will have to come back to fix it later--I have a VERY exciting project to work on that needs my full attention for the next week or so. I will probably discuss that project, and the reason for all of the excitement, in a blog post.


### Built with

- Semantic HTML5 markup
- CSS 3 properties
- JavaScript ES6

### What I learned

- Event Listeners
- Passing Functions as Arguments
- Constructor Functions
- Initialize Object
- Switch Statements
- Methods
- Review of Dot Notation
- Keydown
- Higher Order Functions
- Callbacks
- setTimeout() Method

Wow, I learned so very much during the completion of this project! I took a lot of notes to refer to in the future when I inevitably forget how all of these new things work. My biggest take-away was that even though you may be working with very different data, as long as the arguments passed in are compatible, the same function can be used.  

In this case, we had button click data and keyboard press data to set as our argument. Obtaining the value of the key pressed was straightforward--it was set as one of the values of the event and could be obtained via callback, but the value of the button click had to be created by naming each button the name of a key and then calling that name through innerHTML. In the end, the key press and button click values were identical and were easily passed into the to functions: to play the correct sound and to animate the active selection.  Only having to write two functions shared functions saved an enormous amount of time and lines of code.

Concatenation came into play again during this project in order to pass in the class name, which requires the `.` as in `.w`:

```js
let activeButton = document.querySelector(`.${currentKey}`);
```

It was very interesting to learn the inner workings of addEventListener(), a higher order function, which can take another function as an arugument, and automatically initializes and analyzes an object behind the scenes.

This was an extremely valuable and exciting section!

### Continued development

Unfortunately, the JavaScript sections of this course are not yet updated to ES6, so I am on my own to research how it is done. So far, it has not caused any issues, but I am not yet clear on how and when to use the arrow function. I know that when I get to the REACT Section, ES6 is taught, because I took a sneak peek. Next up for me will be Section 16: The Unix Command Line.  I am skipping jQuery for now so that I can get to Node.js, Express, Databases, APIs and REACT as soon as possible.

### Useful resource

- [fesliyanSTUDIOS.com](https://www.fesliyanstudios.com/royalty-free-sound-effects-download/tom-tom-drums-275) - Here is where I got the sound files for the codepen version.

## Author

Faraja Thompson

- [My Personal Website](https://faraja17.github.io/my-website/)
- [My Blog: Teacher to Techie](https://faraja17.github.io/)
- [Faraja Thompson, M.Ed. on LinkedIn](https://www.linkedin.com/in/faraja-thompson-m-ed-70885b8/)

## Acknowledgments

I'd like to acknowledge my son and mentor [DeForestt Thompson](https://github.com/DeForestt).  His steadfast support and encouragement keep me motivated!  Thanks for forcing me to use the command-line, Son <3 <3 <3.
