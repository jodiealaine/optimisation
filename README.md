## Website Performance Optimization

Optimized this online portfolio for speed! In particular, optimized the critical rendering path and made the page render as quickly as possible.

#### Run the Project

1. Download/clone the repository
2. $> cd /path/to/your-project-folder		
3. $> python -m SimpleHTTPServer 8080		
4. Open a browser and visit localhost:8080		
5. Download and install [ngrok](https://ngrok.com/) to the top-level of your project directory to make your local server accessible remotely.		
6. $> cd /path/to/your-project-folder		
7. $> ./ngrok http 8080		

####Part 1: Optimize PageSpeed Insights score for index.html

- Optimised Images for index.html
- Replaced pizzeria img with an optimised pizzeria-thumbnail
- Inlined CSS
- Asynchronously called JS
- Removed expensive call to web fonts
- Minified CSS, JS and HTML

####Part 2: Optimize Frames per Second in pizza.html

Reduced the script time to generate the last 10 frames:
- Reduced number of sliding pizzas generated
- Moved scrollTop calculation outside of the loop

Reduced time to resize pizzas:
- Moved calculations outside of the loop 
- Refactored calculations to work for one time only and then apply to all

Reduced initial load time:
- Optimed pizzeria image
- Minified CSS, JS and HTML