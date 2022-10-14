# Frontend Mentor - Product preview card component solution

This is a solution to the [Product preview card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/product-preview-card-component-GO7UmttRfa). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

### Links

- Solution URL: [Add solution URL here]( https://github.com/art5551/product_preview_card_component_main.git/)
- Live Site URL: [Add live site URL here]( https://art5551.github.io/product_preview_card_component_main/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox



### What I learned

Easier to code for mobile first
Take the time to setup the colors, fonts, weights and sizes and assign them to variables in the root of the CSS.
Use the following CSS to center content on screen when using flex.

body {
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
}

Use the picture element to make it much easier to code for media queries
<picture>
  <source media="(min-width: 616px)" srcset="images/image-product-desktop.jpg" />
  <img
    src="images/image-product-mobile.jpg"
    alt="picture of a bottle of Gabrielle Essence Eau De Parfum"
  />
</picture>

Very useful to set children to use 50% of the flex container.
Thanks vcarames!
.card-content > * {
  flex-basis: 50%;
}



If you want more help with writing markdown, we'd recommend checking out [The Markdown Guide](https://www.markdownguide.org/) to learn more.

### Continued development



### Useful resources

Several tutorials explaining flex.
Net Ninja and Kevin Powell

## Author

- Website - [Add your name here](https://www.your-site.com)
- Frontend Mentor - [@yourusername](https://www.frontendmentor.io/profile/yourusername)
- Twitter - [@yourusername](https://www.twitter.com/yourusername)


## Acknowledgments

Thanks to vcarames. Was able to gleam alot of information from your project and suggestions.


Kevin Powell
