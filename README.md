The link to the lesson is below:
https://www.codecademy.com/courses/learn-intermediate-css/lessons/css-grid-essentials/exercises/minmax


# GRID ESSENTIALS

## minmax

So far, all of the grids that we have worked with have been a fixed size. The grid in our example has been 400 pixels wide and 500 pixels tall. But sometimes you might want a grid to resize based on the size of your web browser.

In these situations, you might want to prevent a row or column from getting too big or too small. For example, if you have a 100-pixel wide image in your grid, you probably don’t want its column to get thinner than 100 pixels! The minmax() function can help us solve this problem.

```js
.grid {
  display: grid;
  grid-template-columns: 100px minmax(100px, 500px) 100px;
}

```
In this example, the first and third columns will always be 100 pixels wide, no matter the size of the grid. The second column, however, will vary in size as the overall grid resizes. The second column will always be between 100 and 500 pixels wide.


### Instructions
Checkpoint 1 Passed

1. To see minmax() in action, we need to first make the grid have a variable width. Delete the width declaration from .grid.

If you resize your browser, you will see the grid change size with the window.


Hint
The declaration is width: 400px;.

Checkpoint 2 Passed
2. Using minmax(), change the second column to be between 50 pixels and 300 pixels.

Try resizing your browser window. What happens to the other columns when the second column reaches the 300 pixel limit?


Hint
The second column currently has a value 50% width. Replace the value with a minmax() function using 50px as the minimum width and 300px as the maximum width.


memory jog:



/c/Users/glads/Documents/PROJECTS_AT_CODECADEMY/GRID_ESSENTIALS/lesson8_of_15_GRID-ESSENTIALS-minmax
