---
layout: project
type: project
image: images/urinal.jpg
title: peeH
permalink: projects/peeH
# All dates must be YYYY-MM-DD format!
date: 2017-06-01
labels:
  - MITAppInventor
  - Arduino
  - C++
summary: My Sophomore Project that evaluated hydration levels based on urine samples.
---


 Hydration isn't as much advertised around the world. Being hydrated is a key of a healthy life style. My partner and I thought of an invention that would be a simple reminder for people to stay hydrated and drink water.How did we do it? By sticking a pH sensor in to your neighborhood urinals! Your urine actually gives precious data on how your body is doing and knowing if your urine is acidic or basic. This data would be read by a pH sensor and sends the data via Bluetooth to an Android Device. The data that is sent will tell you if you are hydrated or need to go see the doctor.


<img class="ui floated rounded image" src="../images/arduino.png">
 For this project, I was the lead programmer which job was to program the system both in Arduino and MITAppInventor. To begin coding, I had to learn how to code with Arduino and how MITAppInventor works with Arduino. From there, I started researching how a pH sensor works with Arduino and how to code it to be calibrated so it senses the right values based on the liquid that was exposed to it. After the coding for the Arduino was done, I hopped to MITInventor to develop a simple app that will tell the user their dehydration levels based on their urine. We assessed these levels with different types of liquid that would represent a bad pH level (liquid detergent being the low pH and sprite for high pH). This communication was possible with the help of a Bluetooth device that was attached to the Arduino Board that would relay the message to the Android Device. 


 Here is some code that illustrates how we read values from the pH sensor:
<img class="ui medium right floated rounded image" src="../images/mitappinv.png">
<img class="ui medium left floated rounded image" src="../images/code.png">



