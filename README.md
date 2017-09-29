## Website Performance Optimization portfolio project

This project is part of Udacity's frontend nanodegree. The goal is to optimize and improve the performance of a portfolio project.

### Getting started

Click [here](https://rubarammal.github.io/frontend-nanodegree-mobile-portfolio/index.html) to visit the portfolio website. Or clone the project and open `index.html`.

### Optimizations

__* The following changes were applied to `index.html` to improve the performance of the protfolio main page:__

1. The link to `print.css` was removed since the changes in the style were very minor but affected the performance of the page.
1. The link to `style.css` was removed and the style changes were moved to `index.html` inside a `<style>` tag.
1. The link to a google font was removed.
1. A new copy of the __pizzeria.jpg__ image was resized and compressed and moved to the folder __img__ and was used for the project Cam's Pizzeria.
1. All `<script>` tags were moved to the bottom of the page right before the `<body>` closing tag.
1. The keyword `async` was added to `<script src="js/perfmatters.js"></script>`.

__* The following changes were applied to `pizza.html` and `main.js` to improve the performance of Cam's Pizzeria page:__

1. In `changeSliderLabel` function, `pizzaSize` was declared to select `#pizzaSize` id.
1. `changePizzaSizes` was changed to select the size from three fixed sized in percentage and sets the new size of pizzas by looping on `randomPizza` which is an array of all the elements in the class `randomPizzaContainer`.
1. `var pizzasDiv = document.getElementById("randomPizzas");` was moved out of the loop.
1. In `updatePositions`, `scrollTop` was moved out of the for loop.
