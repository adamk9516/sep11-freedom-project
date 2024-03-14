# Entry 3
##### 2.11.24

### Context
The past few weeks I have learned how to label the x and y axes on a bar graph and how to create a pie chart. I watched the video [Let's learn D3.js - D3 for data visualization (full course)](https://www.youtube.com/watch?v=C4t6qfHZ6Tw) by [freeCodeCamp](https://freeCodeCamp.org). The man in the video taught me how to label the axes of a graph and how to create a pie chart.

### EDP
I am still currently on step 4 of the Engineering Design Process which is to brainstorm possible solutions to my problem of visualizing baseball data. The next part of the EDP is to create a prototype. I will start by compiling all of the formulas for my data. Then I will add text boxes for answers. I will work towards my MVP by May 1st.

### Skills
During this time I have learned some valuable skills that not only help me with coding but also with other things such as having a growth mindset. Coding is extreamly hard and you need to have a specific mindset when doing so. You have to be prepared to fail time and time again before you succeed. For example, when my class was learning loops for the first time, many of us crashed our browsers because we created infinit loops. Through practice and time spent working on this skill we were able to make loops without crashing out browsers. Connecting back to learning D3.js, when first trying to create a pie chart I went to refresh my page and it was blank. I felt so defeated because I spent a good amount of time working to make the pie chart.

Another skill I learned was problem decomposition. When I was starting to code my first bar chart there was so much that went into it and thinking about it as a whole drove me crazy. So I broke the chart down into smaller pieces and took the time to really learn what `.attr`, `.call`, `.append`, and `.ticks` were and how they worked together.

## Axes Labels
### x-axis
The x axis in this case will show "NAMES" and will be positioned horizontally based on the width of the graph and vertically based on the height of the graph minus 6.
``` js
svg.append("text")
  .attr("class", "x label")
  .attr("text-anchor", "end")
  .attr("x", width)
  .attr("y", height - 6)
  .text("NAMES");
```
### y-axis
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
## Pie Chart Data
This dataset shows the different parts of data and also how percentage of space they take up in the graph
``` js

var data = [
  {"platform": "Android","percentage": 40.11},
  {"platform": "Windows","percentage": 36.69},
  {"platform": "iOS","percentage": 13.06}
];
```
### MVP

I am getting started on my MVP. I started by compiling all of my formulas for collecting data. The goal for the project is for people to type their own statistics such as how many hits they have and how many at-bats they have. Then the code website would output their average(how many hits divided my the number of at-bats).

##### Hitting

##### Batting avg - Hits / At-bats = 3 decimals

##### On-base Percentage - (Hits + Walks + Hit By Pitch) / (At-bats + Walks + Hit By Pitch + Sacrifices) = 3 decimals

##### Slugging Percentage - Total number of bases / At-bats

##### On-base plus Slugging - On-base percentage + Slugging percentage


##### Pitching

##### Earned Run Average - (Earned Runs Allowed) / (Innings Pitched) * 9




[Previous](entry02.md) | [Next](entry04.md)

[Home](../README.md)
