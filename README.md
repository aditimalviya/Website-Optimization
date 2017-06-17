# This is a website optimisation project. The task is to optimize a given website so that it reaches a target score at PageSpeed Insights and frames per second rate of 60fps.

## Part1: PageSpeed Score

*Target*
The target was to make index.html reach 90 or higher score for Mobile & Desktop at PageSpeed Insights.

*Optimization*

1. Inline style.css
2. Async analytics.js and scripts to load google fonts.
3. Compress pizzeria.jpg as it is 2.4MB.
4. Minimize html, css, scripts & all images.

##Part 2: Getting Rid of Jank

*Target*

1.Make views/pizza.html reach 60 fps rate when scrolling.
2.Make time to resize pizzas less than 5ms.

*Optimization*

1. When you use timeline, spot two functions ( changePizzaSizes(), updatePositions()) that have forced synchronous layout in them.
2. In changePizzaSizes(), get rid of the time consuming for loop by calculating the new width out of the loop only once.
3. In updatePositions(), move the causing layout line out of the loop.

*How to run this project locally*
Open index.html in your browser.