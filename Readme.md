# Task 7: CSS Responsive Issues (Media Queries & Variables)

**Author:** D P Rithvik Kumar

## Description & Learning Process
In this task, I reworked the Laundry Services Hero section to be fully responsive across desktop, tablet, and mobile views using Flexbox and Media Queries. 

I learned a lot during this iteration. Initially, I made the mistake of applying `flex-direction: column` too early at the tablet breakpoint. I realized that a tablet screen is still wide enough to handle a side-by-side (`row`) layout, so I updated the 1024px media query to simply shrink the fonts and image sizes instead. I saved the `flex-direction: column` stacking exclusively for the mobile breakpoint (768px). 

I also experimented with CSS Variables (`:root`). I successfully used them to manage my color palette, but I ran into a roadblock when I tried to use a variable for my `@media (max-width: var(--mobile-bp))` rule. After some troubleshooting, I learned that standard CSS doesn't actually allow variables inside media query declarations yet! Finally, I added a global `transition` property so the website smoothly scales instead of harshly snapping when you resize the browser window.

## How to Run
1. Download or clone this repository to your computer.
2. Make sure `index.html` and `style.css` are in the same folder.
3. Open `index.html` in any web browser.
4. Slowly drag the edge of your browser window to make it smaller. Watch how the elements smoothly scale down for tablet mode, and then eventually stack vertically into a column for mobile mode.
