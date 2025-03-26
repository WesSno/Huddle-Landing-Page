# Frontend Mentor - Huddle landing page with curved sections solution

This is a solution to the [Huddle landing page with curved sections challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/huddle-landing-page-with-curved-sections-5ca5ecd01e82137ec91a50f2). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
- [Author](#author)
- [Acknowledgments](#acknowledgments)

**Note: Delete this note and update the table of contents based on what sections you keep.**

## Overview

### The challenge

Users should be able to:

- View the optimal layout for the site depending on their device's screen size
- See hover states for all interactive elements on the page

### Links

- Solution URL: [GitHub](https://github.com/WesSno/Huddle-Landing-Page)
- Live Site URL: [Add live site URL here](https://your-live-site-url.com)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- Mobile-first workflow
- Inline Vanilla JavaScript

### What I learned

I learned that the default browser validation can be removed by changing **type="email"** into **type="text"** and handling the default behaviour of the form tag.

To see how you can add code snippets, see below:

```html
<input
  type="text"
  name="email"
  id="email"
  placeholder="Enter your email"
  required
/>
```

```js
function checkEmail() {
  event.preventDefault();
  const emailInput = document.getElementById("email").value;
  const emailBox = document.querySelector("input[type='text']");
  let errMsg = document.getElementsByClassName("error-msg")[0];

  if (emailValidation(emailInput)) {
    errMsg.classList.remove("display-err");
    emailBox.classList.remove("border-color");
  } else {
    errMsg.classList.add("display-err");
    emailBox.classList.add("border-color");
  }
}
```

I also learned how to change the default color of a logo using the code below:

```css
.contact-info .logo {
  filter: invert(100%) sepia(100%) brightness(1000%) contrast(100%);
  width: 70%;
  margin-bottom: 1em;
}
```

## Author

- Website - [Kofi Baafi Kwatia](https://github.com/WesSno)
- Frontend Mentor - [@yourusername](https://www.frontendmentor.io/profile/yourusername)
