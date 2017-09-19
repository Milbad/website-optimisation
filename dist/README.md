## Website Performance Optimization portfolio project ##

In this project I had to optimize an online portfolio for speed! In particular, optimize the critical rendering path and make this page render as quickly as possible by applying the techniques I have picked up in the [Critical Rendering Path course](https://www.udacity.com/course/ud884).

### Getting started ###

1. Unzip the Website Optimization directory.
2. Open the dist directory.
3. Launch the index.html file

### Optimization Made
#### Generalities #### 
1. Compress and resize images
2. Minify css and javascript files

#### In the index.html file ####
1. Inline style.css
2. Remove google font url
3. Add the async attribute to the google analytic script
4. Create a portrait.css file
5. Add a media query to portrait.css and print-min.css

#### In the main.js file ####
1. Change querySelectorAll for getElementsByClassName or getElementById
2. In the UpdatePosition function, create a variable top to store document.body.scrollTop outside of the for loop 
3. In changePizzaSizes(), move newwidth and dx variables outside of the for loop
4. In changePizzaSizes(), create the random variable outside of the loop to store the DOM element
5. Move variables items, phase, i and l outside of the UpdatePosition loop
6. In the UpdatePosition function, create 2 loops. 1 to calculate phase and the other to update the style of each item
7. Reduce the number of sliding pizzas regarding the height of the window
8. Row 528: declare the variable elem outside of the for loop

#### In the pizza.html file ####
1. Inline the style.css file
2. use bootstrap-grid-min.css instead of bootstrap-grid.css