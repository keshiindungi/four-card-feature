# Four Card Feature Section

This is a solution to the [Four card feature section challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/four-card-feature-section-weK1eFYK). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

## Table of Contents

- [Overview](#overview)
  - [The Challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My Process](#my-process)
  - [Built With](#built-with)
  - [What I Learned](#what-i-learned)
  - [Continued Development](#continued-development)
- [Author](#author)

## Overview

### The Challenge

Users should be able to:

- View the optimal layout for the site depending on their device's screen size.

### Screenshot

![](./design/desktop-preview.jpg)

### Links

- Solution URL: [Add your solution URL here](https://your-solution-url.com)
- Live Site URL: [Add your live site URL here](https://your-live-site-url.com)

## My Process

### Built With

- Semantic HTML5 markup
- CSS Custom Properties
- Flexbox
- CSS Grid
- Mobile-first workflow
- [Poppins](https://fonts.google.com/specimen/Poppins) - Google Font

### What I Learned

This project was an excellent exercise in using CSS Grid for 2D layouts. The main challenge was achieving the staggered card effect on desktop while maintaining a clean stacked layout on mobile.

I used `grid-template-columns` and `grid-row` properties to position the cards precisely:

```css
.features-grid {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  grid-template-rows: repeat(2, 1fr);
  align-items: center;
}

.card-supervisor {
  grid-column: 1;
  grid-row: 1 / span 2;
}
```

This allowed the "Supervisor" and "Calculator" cards to span across two rows, effectively centering them vertically relative to the middle column.

### Continued Development

In the future, I plan to:
- Add minor animations to the cards on hover (e.g., slight lift effect).
- Improve accessibility by verifying contrast ratios and focus states.

## Author

- Website - [Your Name](https://www.your-site.com)
- Frontend Mentor - [@yourusername](https://www.frontendmentor.io/profile/yourusername)
