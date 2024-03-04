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
03/03/2024
This past week I learned how to make a pie chart and how to input data into it using percentages. I also learned how to size the chart so it isn't too big that it takes up the whole webpage but isn't too small that it can't be seen.

``` js
var data = [
  {"platform": "Android","percentage": 40.11},
  {"platform": "Windows","percentage": 36.69},
  {"platform": "iOS","percentage": 13.06}
];
```
All the percentages add up to 100 to fill the whole area of the pie chart.
``` js
var svgWidth = 500, svgHeight = 300, radius = Math.min(svgWidth, svgHeight) / 2;
var svg = d3.select('svg')
  .attr("width", svgWidth)
  .attr("height", svgHeight);
```
This will take the smallest number using `Math.min` and divide it by two to get the radius of the pie chart.

My next step is to make the pie chart adaptable so when the user puts in their own data, they can have a pie chart with their own data.
<!--
* Links you used today (websites, videos, etc)
* Things you tried, progress you made, etc
* Challenges, a-ha moments, etc
* Questions you still have
* What you're going to try next
-->
