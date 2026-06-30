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
- [Author](#author)

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

Since I've recently just learned to use semantic elements, I know that my use of the **`<figcaption>`** element is quite off. Instead, it must be a direct child of the **`<figure>`** element. Therefore, I want to dive much deeper into the appropriate uses of semantic elements for the sake of my future developments.

With research, I also found out that I should've used the **`<img>`** element for embedding the QR code in my page, rather than use the **`background`** CSS property. That is because the QR code acts as content, rather than a background design, meaning **`<img>`** suits this case better. Here is what my HTML structure should have been:

```html
<main>
  <article class="card"">
    <figure class="qr-code-container">
      <img src="./images/image-qr-code-png" alt="QR Code to Frontend Mentor">
      <figcaption class="card-info">
        <p>Improve your front-end skills by building projects</p>
        <p>Scan the QR code to visit Frontend Mentor and take your coding skills to the next level</p>
      </figcaption>
    </figure>
  </article>
</main>
```

I do not plan on fixing this semantic issue yet, as this mini-project just serves as my practice. But I might do so in the future.

Not only that, my [styles.css](styles.css) lacked CSS variables which I want to explore more in the future, especially its best practices for when to use it.

### Useful resources

- [Transfonter.org](https://transfonter.org/) - This tool allowed me convert font files from TTF to WOFF/WOFF2 to optimize website performance. Refer to [Google web.dev: Optimize Web Fonts](https://web.dev/learn/performance/optimize-web-fonts) for more information.
- [MDN - Background CSS Property](https://developer.mozilla.org/en-US/docs/Web/CSS/Reference/Properties/background) - This document about the **`background`** property helped me understand the correct syntax.

## Author

- Frontend Mentor - [Jacob Titong](https://www.frontendmentor.io/profile/jacobtitong)
