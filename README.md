# NativeJS-timer
Timer on Native JS
To use this timer you need.
1. To create variable with final date
2. To have an html container for your timer with id '#timer'.
3. To have html elements with classes:
  .days for days
  .hours for hours
  .minutes for minutes
  .seconds for seconds

How this works?

We have  variables:
1. variable for final date
2. variable for container
3. variables for days, hours, minutes, seconds 

We have 2 functions.
1. getTimeRemaining that counts time from now to final date and returns it in object
2. setClock that sets our timer and have an inner function updateClock
  that calls function getTimeRemaining, gets object elements from it and puts this elements into html blocks


If you want to create an opposite timer that counts from variable date to current date just change variable t to t = Date.parse(new Date()) - Date.parse(endtime)
