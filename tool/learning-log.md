# Tool Learning Log

Tool: **D3**

Project: **Baseball Stats**

---

10/29/2023:
* I started to watch a video called [Data Visualization with D3, JavaScript, React - Full Course [2021]](https://www.youtube.com/watch?v=2LhoCfjm8R4)

11/26/2023:
* This week I learned how to create a dataset and print it out using D3.js

12/17/2023:
* This week I learned how to set the scales for the x and y axes
const x = d3.scaleTime()
.range([0, width]);

const y = d3.scaleLinear()
.range([height, 0]);

02/10/2024
* This week I learned how to label the x and y axes. I watched [Let's learn D3.js - D3 for data visualization (full course)](https://www.youtube.com/watch?v=C4t6qfHZ6Tw) by FreeCodeCamp and they taught me how to label the axes.

The x axis in this case will show "NAMES" and will be positioned horizontally based on the width of the graph and vertically based on the height of the graph minus 6.

``` js
svg.append("text")
  .attr("class", "x label")
  .attr("text-anchor", "end")
  .attr("x", width)
  .attr("y", height - 6)
  .text("NAMES");
```
The y axis will show "SCORES (/100)" and will be rotated 90 degrees counter-clockwise so it lines up with the left side of the graph. It will be vertically based on the height minus 375.

``` js
svg.append("text")
  .attr("class", "y label")
  .attr("text-anchor", "end")
  .attr("y", height - 375)
  .attr("tranform", "translate(-40, 40)")
  .attr("dy", ".75em")
  .attr("transform", "rotate(-90)")
  .text("SCORES (/100)");
```
<!--
* Links you used today (websites, videos, etc)
* Things you tried, progress you made, etc
* Challenges, a-ha moments, etc
* Questions you still have
* What you're going to try next
-->
