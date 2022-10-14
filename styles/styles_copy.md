/* fonts supplied by the style guide */

@font-face {
  font-family: Montserrat;
  src: url(https://fonts.google.com/specimen/Montserrat);
}

/* colors provided in the style guide */
:root {
  --very-dark-blue: hsl(212, 21%, 14%);
  --dark-grayish-blue: hsl(228, 12%, 48%);
  --white: hsl(0, 0%, 100%);
  --dark-cyan: hsl(158, 36%, 37%);
  --cream: hsl(30, 38%, 92%);

  --font-family-accent: 'Fraunces', serif;
  --font-family-body: 'Montserrat', sans-serif;
}

@media (min-width: 50em) {
  :root {
    /* set the regular fonts in the main root and set them again here for mobile*/
    --fs-400: 1rem;
  }
}


/* Beginning of reset CSS with minor changes recommended by Kevin Powell */
/* see youtube https://www.youtube.com/watch?v=h3bTwCqX4ns */
/* Box sizing rules */
*,
*::before,
*::after {
  box-sizing: border-box;
}

/* Remove default margin */
* {
  margin: 0;
  padding: 0;
  font: inherit;
}

/* Remove list styles on ul, ol elements with a list role, which suggests default styling will be removed */
ul[role='list'],
ol[role='list'] {
  list-style: none;
}

/* Set core root defaults */
html:focus-within {
  scroll-behavior: smooth;
}

/* Deviation from KPowell*/
html,
body {
  height: 100%;
}

/* Set core body defaults */
body {
  text-rendering: optimizeSpeed;
  line-height: 1.5;
}

/* A elements that don't have a class get default styles */
a:not([class]) {
  text-decoration-skip-ink: auto;
}

/* Make images easier to work with */
img,
picture,
svg {
  max-width: 100%;
  display: block;
}

/* Remove all animations, transitions and smooth scroll for people that prefer not to see them */
@media (prefers-reduced-motion: reduce) {
  html:focus-within {
   scroll-behavior: auto;
  }
  
  *,
  *::before,
  *::after {
    animation-duration: 0.01ms !important;
    animation-iteration-count: 1 !important;
    transition-duration: 0.01ms !important;
    scroll-behavior: auto !important;
  }
}
/* End of reset CSS*/

.attribution { 
  font-size: 11px; text-align: center; 
}
.attribution a { 
  color: hsl(228, 45%, 44%); 
}

.container {  
  --max-width: 1440px;
  --padding: 1rem;

  width: min(var(--max-width), 100% - (var(--padding) * 2));
  margin-inline: auto;
  background-color: var(--cream);
  justify-content: center;

}

.even-columns {
  max-width: 200;
  height: 700vh;
  display: grid;
}

@media (min-width: 50em) {
  .even-columns {
    grid-auto-flow: column;
    grid-auto-columns: 1fr;
  }
}

.product-header {
  color: var(--very-dark-blue);
  font-family: var(--font-family-body);
  font-weight: 700;
  font-size: 22px;
  letter-spacing: 5px;
}

.product-title {
  color: var(--very-dark-blue);
  font-family: var(--font-family-accent);
  font-weight: 700;
  font-size: 24px;
}

.product-description {
  color: var(--very-dark-blue);
  font-family: var(--font-family-body);
  font-weight: 500;
}

/* @media only screen and (max-width: 400px) {
  .card {
    border-radius: 25px;
    display: flex;
    flex-wrap: wrap;
    align-items: center;
    justify-content: center;
    flex-direction: column;
  }
} */