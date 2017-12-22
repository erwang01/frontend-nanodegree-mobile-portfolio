## Website Performance Optimization portfolio project

### Changes Made
- Reduce size of pizzeria.jpg to 100px; file named to pizzeria100.jpg and placed in img/
- Compress pizzeria100.jpg and profilepic.jpg 75% quality, new file names pizzeria10075.jpg and profilepic75.jpg
- Made all print styles async along with analytic scripts.
- Removed Open Sans Font due to long download times
- Added media tag to print.css
- Removed README.md from dist/
- Added optimized image,JS, and CSS resources to dist/, keeping originals in src/
- Moved all images onto repository, no longer dependent on remote servers.

main.js optimizations:
- Moved scrollTop query to outside of the for loop.
- Removed dx calculations from changing pizza size, combined it into changingPizzaSizes method.
- Moved pizza icon query out of the for loop.
- Used document.getElementById instead of querySelector.
- Used document.getElementsByClassName instead of querySelectorAll
- Moved pizzasDiv outside of the loop.
- Moved movingPizzas query out of the loop.
- Declare variables out of the loop.

views/css/style.css changes:
- added transformZ(0); to moving pizzas.

### Getting started

  ```bash
  $> cd /path/to/your-project-folder
  $> python -m SimpleHTTPServer 8080
  ```

1. Open a browser and visit localhost:8080
1. ngrok to make your local server accessible remotely.

  ``` bash
  $> cd /path/to/your-project-folder
  $> ./ngrok http 8080
  ```
