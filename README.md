# Frontend Mentor - Fylo data storage component solution

This is a solution to the [Fylo data storage component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/fylo-data-storage-component-1dZPRbV5n). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
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

- View the optimal layout for the site depending on their device's screen size

### Screenshot

![Fylo data storage component](./screenshot.jpg)

### Links

- Solution URL: [https://github.com/shElkhateeb/fylo-data-storage-component-master](https://github.com/shElkhateeb/fylo-data-storage-component-master)
- Live Site URL: [https://shelkhateeb.github.io/fylo-data-storage-component-master/](https://shelkhateeb.github.io/fylo-data-storage-component-master/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox

### What I learned

- How to style an input of type file

```html
<label for="upload" class="box" role="button" title="Upload file">
  <img src="./images/icon-upload.svg" alt="Upload" />
  <input type="file" id="upload" />
</label>
```

```css
header .icons .box input[type="file"] {
  display: none;
}
```

- Style progress bar

``` css
progress {
  appearance: none;
  -moz-appearance: initial;
  background: var(--color-very-dark-blue);
  width: 100%;
  height: 1rem;
  border: none;
  border-radius: 0.5rem;
  -webkit-border-radius: 0.5rem;
  -moz-border-radius: 0.5rem;
  -ms-border-radius: 0.5rem;
  -o-border-radius: 0.5rem;
  border: solid 2px var(--color-very-dark-blue);
  position: relative;
}
/* webkit */
progress::-webkit-progress-bar {
  background: var(--color-very-dark-blue);
  border-radius: 0.5rem;
  -webkit-border-radius: 0.5rem;
  -ms-border-radius: 0.5rem;
  -o-border-radius: 0.5rem;
}
progress::-webkit-progress-value {
  background: linear-gradient(
    to right,
    var(--color-gradient-from),
    var(--color-gradient-to)
  );
  border-radius: 0.5rem;
  -webkit-border-radius: 0.5rem;
  -ms-border-radius: 0.5rem;
  -o-border-radius: 0.5rem;
}
/* firefox */
progress::-moz-progress-bar {
  background: linear-gradient(
    to right,
    var(--color-gradient-from),
    var(--color-gradient-to)
  );
  border-radius: 0.5rem;
  -moz-border-radius: 0.5rem;
}
```

### Useful resources

- [Making Responsive Images With CSS Properties](https://www.bitdegree.org/learn/responsive-image#setting-background-size-to-fit-screen) - This helped me for setting the back ground image.
- [Creating A Custom Range Input That Looks Consistent Across All Browsers](https://www.smashingmagazine.com/2021/12/create-custom-range-input-consistent-browsers/) - This is an amazing article which helped me finally understand how to customize range input and progress bar. I'd recommend it to anyone still learning this concept.
- [How you can style the input file type in forms using CSS](https://www.educative.io/answers/how-you-can-style-the-input-file-type-in-forms-using-css) - This helped me to make the upload button.

## Author

- Frontend Mentor - [@shElkhateeb](https://www.frontendmentor.io/profile/shElkhateeb)
