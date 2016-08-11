## Website Performance Optimization

####Part 1: Optimize PageSpeed Insights score for index.html

- Optimised Images for index.html
- Replaced pizzeria img with an optimised pizzeria-thumbnail
- Inlined CSS
- Asynchronously called JS
- Removed expensive call to web fonts
- Minified CSS, JS and HTML

####Part 2: Optimize Frames per Second in pizza.html

- Reduced the script time to generate the last 10 frames:
-- Reduced number of sliding pizzas generated
-- Moved scrollTop calculation outside of the loop

- Reduced time to resize pizzas:
-- Moved calculations outside of the loop 
-- Refactored calculations to work for one time only and then apply to all

- Reduced initial load time:
-- Optimed pizzeria image
-- Minified CSS, JS and HTML