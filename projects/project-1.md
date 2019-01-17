---
layout: project
type: project
image: images/urinal.jpg
title: peeH
permalink: projects/peeH
# All dates must be YYYY-MM-DD format!
date: 2015-07-01
labels:
  - MITAppInventor
  - Arduino
  - C++
summary: My Sophomore Project that evaluated hydration levels based on urine samples.
---

<div class="ui small rounded images">
  <img class="ui image" src="../images/micromouse-robot.png">
  <img class="ui image" src="../images/micromouse-robot-2.jpg">
  <img class="ui image" src="../images/micromouse.jpg">
  <img class="ui image" src="../images/micromouse-circuit.png">
</div>

Hydration and b
Micromouse is an event where small robot “mice” solve a 16 x 16 maze.  Events are held worldwide.  The maze is made up of a 16 by 16 gird of cells, each 180 mm square with walls 50 mm high.  The mice are completely autonomous robots that must find their way from a predetermined starting position to the central area of the maze unaided.  The mouse will need to keep track of where it is, discover walls as it explores, map out the maze and detect when it has reached the center.  having reached the center, the mouse will typically perform additional searches of the maze until it has found the most optimal route from the start to the center.  Once the most optimal route has been determined, the mouse will run that route in the shortest possible time.

For this project, I was the lead programmer which job was to program the system both in Arduino and MITAppInventor. To begin coding, I had to learn how to code with Arduino and how MITAppInventor works with Arduino. From there, I started researching how a pH sensor works with Arduino and how to code it in order to be calibrated so it senses the right values based on the liquid that was exposed to it. After the coding for the Arduino was done, I hopped to MITInventor to create a simple app that will tell the user their dehydration levels based on their urine. We tested these levels with different types of liqiud that would represent a bad pH levels (liqiuid detergent being the low pH and sprite for high pH). This communication was possible with the help of a bluetooth device that was attached to the Arduino Board that would relay the message to the Andriod Device. 

Here is some code that illustrates how we read values from the line sensors:

```js
byte ADCRead(byte ch)
{
    word value;
    ADC1SC1 = ch;
    while (ADC1SC1_COCO != 1)
    {   // wait until ADC conversion is completed   
    }
    return ADC1RL;  // lower 8-bit value out of 10-bit data from the ADC
}
```

You can learn more at the [UH Micromouse Website](http://www-ee.eng.hawaii.edu/~mmouse/about.html).



