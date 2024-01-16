# Entry 2
##### 12.17.23

I am still on part 4 of the Engineering Design Process(EDP) which is planning on how to solve my issue. Through this time I have learned some valuable skills. Skills such as my creativity and attention to detail. When working with many numbers you don't always know exatly what they mean or do, sometimes you have to change them to see what changes in the result. 

This past week I have learned how to set the x and y axes for a graph and I can create a dataset that gets printed in graphical form. I watched [D3.js Tutorial - Making a Bar Chart Graph
](https://www.youtube.com/watch?v=BDpBAFvdjYo&t=670s) by Kris Foster where he walked me through how to make a bar graph using D3.js. His video explained how each component worked together to make the graph. I followed along, copying everything in the video. After I finished the video I played around with the numeric values in the code to see what they do and what they change.
``` js
const data = [
  { name: 'Adam', score:92 },
  { name: 'Shelly', score:55 },
  { name: 'Mueller', score:77 },
  { name: 'Daniel', score:100 },
  { name: 'Dong', score:65 },
  { name: 'William', score:50 },
  { name: 'Stefanie', score:84 },
];
```
The first part of each piece of data is the x-axis. For example Adam or Mueller. and the score is the y-axis 92 or 77. 

``` js
const width = 800;
const height = 400;
const margin = { top: 50, bottom: 50, left: 50, right:50};
```
Width describes the size going from left to right and height describes the size going up and down. The margin describes the size between the edge of the screen and the graph. 

### Scale 

``` js
const x = d3.scaleBand()
  .domain(d3.range(data.length))
  .range([margin.left, width - margin.right])
  .padding(0.05);
```
``` js
const y = d3.scaleLinear()
  .domain([0, 100])
  .range([height - margin.bottom, margin.top])

```
.scaleLinear creates a scale for the graph and makes it proportional to the output/linear.

### Next Steps

My next steps for the freedom project are to put my learning of D3.js into use in my project by practicing coding the visualization of data within my topic of baseball statistics. Coding with this specific topic in mind will help me when it comes to coding the actual project because I will have experience with it and it will be more familiar 
[Previous](entry01.md) | [Next](entry03.md)

[Home](../README.md)
