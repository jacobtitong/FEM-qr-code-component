# Frontend Mentor - QR code component solution

This is a solution to the [QR code component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/qr-code-component-iux_sIO_H). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

## Table of contents

- [Overview](#overview)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
  - [Useful resources](#useful-resources)
  - [AI Collaboration](#ai-collaboration)
- [Author](#author)
- [Acknowledgments](#acknowledgments)

**Note: Delete this note and update the table of contents based on what sections you keep.**

## Overview

### Screenshot

![Desktop Design](./screenshots/desktop-design.png)
![Mobile Design](./screenshots/mobile-design.png)

### Links

- Solution URL: [Github Repository](https://github.com/jacobtitong/FEM-qr-code-component)
- Live Site URL: [Live Github Page](https://jacobtitong.github.io/FEM-qr-code-component/)

## My process

### Built with

- HTML & CSS
- Semantic HTML5 markup
- Flexbox
- Mobile-first workflow
- Google Fonts

### What I learned

For HTML, I learned that semantic markup is incredibly important for accessibility and support for screen readers. I implemented this practice using four semantic HTML elements (excluding the already-provided footer). **`<main>`** indicates the primary content of the page. **`<article>`** is a section of a page that is reusable, meaning it can be implemented multiple times across different web pages. In this case, article is the QR code component or card. **`<figure>`**, by the word itself, indicates any kind of visual element or illustration which is the QR code itself. While **`<figcaption>`** represents the contents describing the QR code figure.

```html
<main>
  <article class="card"">
    <figure class="qr-code">
    </figure>
    <figcaption class="card-info">
      <p>Improve your front-end skills by building projects</p>
      <p>Scan the QR code to visit Frontend Mentor and take your coding skills to the next level</p>
    </figcaption>
  </article>
</main>
```

As for CSS, one of the technical things I have ever done for this solution is making the custom google fonts to work with my text. I understand that you can link the external fonts directly into HTML, however, I also considered the possibility of the external font to fail in connecting to my website. Which is why I had to download it and convert it into woff/woff2 for quick and easier access.

```css
@font-face {
  font-family: "Outfit";
  src:
    url("fonts/Outfit-Bold.woff2") format("woff2"),
    url("fonts/Outfit-Bold.woff") format("woff");
  font-weight: bold;
  font-style: normal;
  font-display: swap;
}

@font-face {
  font-family: "Outfit";
  src:
    url("fonts/Outfit-Regular.woff2") format("woff2"),
    url("fonts/Outfit-Regular.woff") format("woff");
  font-weight: normal;
  font-style: normal;
  font-display: swap;
}
```

### Continued development

Use this section to outline areas that you want to continue focusing on in future projects. These could be concepts you're still not completely comfortable with or techniques you found useful that you want to refine and perfect.

**Note: Delete this note and the content within this section and replace with your own plans for continued development.**

### Useful resources

- [Example resource 1](https://www.example.com) - This helped me for XYZ reason. I really liked this pattern and will use it going forward.
- [Example resource 2](https://www.example.com) - This is an amazing article which helped me finally understand XYZ. I'd recommend it to anyone still learning this concept.

**Note: Delete this note and replace the list above with resources that helped you during the challenge. These could come in handy for anyone viewing your solution or for yourself when you look back on this project in the future.**

### AI Collaboration

Describe how you used AI tools (if any) during this project. This helps demonstrate your ability to work effectively with AI assistants.

- What tools did you use (e.g., ChatGPT, Claude, GitHub Copilot)?
- How did you use them (e.g., debugging, generating boilerplate, brainstorming solutions)?
- What worked well? What didn't?

**Note: Delete this note and the content above if you didn't use AI, or replace with your own experience.**

## Author

- Website - [Add your name here](https://www.your-site.com)
- Frontend Mentor - [@yourusername](https://www.frontendmentor.io/profile/yourusername)
- Twitter - [@yourusername](https://www.twitter.com/yourusername)

**Note: Delete this note and add/remove/edit lines above based on what links you'd like to share.**

## Acknowledgments

This is where you can give a hat tip to anyone who helped you out on this project. Perhaps you worked in a team or got some inspiration from someone else's solution. This is the perfect place to give them some credit.

**Note: Delete this note and edit this section's content as necessary. If you completed this challenge by yourself, feel free to delete this section entirely.**
