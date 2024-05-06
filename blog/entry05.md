# Entry 5
##### 05/05/2024

### EDP
Last week I was on step 6 of the Engineering Design process which is to test and evaluate my product. I submitted my MVP and I am now on step 7 of the EDP which is to Improve my product. My goal in step 7 is to make my product look professional by changing the background, changing the font, and changing the color and position of the pie chart.

### Finishing MVP
I added 4 new prompts for the user to calculate their baseball statistics. They are strikeout rate, walk rate, homerun ratio, and batting average against. Each is coded the same way and I reused variables in multiple different prompts. The way a user picks which statistic they want to calculate is by pressing a certain letter on the keyboard. For example,

``` js
}else if (event.keyCode === 83) {
  var strikeOuts = prompt('How many strikeouts do you have?')
  var hitters = prompt('How many hitters have you faced?')
  var strikeoutRate = strikeOuts / hitters;
  document.write('Your strikeout percentage is ' + Math.round(strikeoutRate * 100) + '%')
```
This code contains an if statement with an event saying if 'S' is pressed the rest of the code will run. If the key is pressed then the user will be prompted to answer 2 questions and then the user will get their strike out percentage.


[Previous](entry04.md) | [Next](entry06.md)

[Home](../README.md)
