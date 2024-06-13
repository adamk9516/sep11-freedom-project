# Entry 5
##### 05/05/2024

### EDP
Last week I was on step 6 of the Engineering Design process which is to test and evaluate my product. I submitted my MVP and I am now on step 7 of the EDP which is to Improve my product. My goal in step 7 is to make my product look professional by changing the background, changing the font, and changing the color and position of the pie chart.

### Finishing MVP

I Added my pie chart to my calculator but noticed it was too large. I had other things on the screen and the pie chart didn't fit. I knew that to make it smaller, I had to define the width and height. I made them both 400px and made the radius half because width or height would be the diameter of the circle.
``` js
const width = 400;
const height = 400;
const radius = Math.min(width, height) / 2;
```
I also added 4 new prompts for the user to calculate their baseball statistics. They are strikeout rate, walk rate, homerun ratio, and batting average against. Each is coded the same way and I reused variables in multiple different prompts. The way a user picks which statistic they want to calculate is by pressing a certain letter on the keyboard. For example,

``` js
}else if (event.keyCode === 83) {
  var strikeOuts = prompt('How many strikeouts do you have?')
  var hitters = prompt('How many hitters have you faced?')
  var strikeoutRate = strikeOuts / hitters;
  document.write('Your strikeout percentage is ' + Math.round(strikeoutRate * 100) + '%')
```
While learning how to best round my numbers I knew that for some of them I needed to decimal places. For example, for ERA (Earned Run Average) is always rounded to the hundredth. I used a fourm called [Rounding to the nearest hundredth of a decimal in JavaScript](https://stackoverflow.com/questions/14968615/rounding-to-the-nearest-hundredth-of-a-decimal-in-javascript) which helped me to learn that however many decimal places I want is the number of zeros that I have to multiply and divide. For example. `(num * 100) / 100`

This code contains an if statement with an event saying if 'S' is pressed the rest of the code will run. If the key is pressed then the user will be prompted to answer 2 questions and then the user will get their strike out percentage.

One skill I learned during this process was the skill of knowing how to google. It is very easy to get lost in a google search and not be able to find what you are looking for. You have to know where to look and you need to know how to read fourms because especially with Javascript, most of the help you need is in fourms. 

Another skill I learned was how to read. For the same reason as how to google, this skill is important because if you dont understand how to go through a fourm, then you will never find what you are looking for. 


[Previous](entry04.md) | [Next](entry06.md)

[Home](../README.md)
