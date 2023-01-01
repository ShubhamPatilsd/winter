---
name: "@ShubhamPatilsd"
project: "ArrowNav"
---

# ArrowNav

## Summary

ArrowNav is a giant wooden arrow that you can put on your bike to navigate to where you want to go!

## Plan
Ok so the big arrow will be attached to 360 degree servo that rotates and points in a certain heading. The RPi/computer will be attached to the arrow. On the RPi will be a magnetometer, which can tell me the heading of where the RPi is facing (which I can use to tell the servo how much to rotate). Jason on the Slack helped me resolve my issues. ~~I'm still asking about how to get the servo to point in a certain direction in the Hack Club Slack, but I am sure that it will be acheivable in some way.~~ 

To get navigation data, I'm going to be using [Mapbox's APIs](https://docs.mapbox.com/api/navigation/directions/) to get the route data. The route data includes the major "turn points" including coordinates and the heading I should be in after the turn. I will be using this API for free for 100,000 requests, and only at the start of a trip. I will be connecting to my phone's mobile data, and I will only need to make a request once (at the start). After that, the route will be cached until a new trip is started. 

I will also use a GPS module for the RPi to get the current latitude and longitude, so I can see if I'm in a 15 meter distance of an intersection so that I can move the servo to avoid confusion. The Mapbox API has coordinates for where each turn takes place!

## Budget

What materials will you need for your project? Where will you get them? How much does it cost? Please include all materials, including components you already own. Make sure to factor in shipping costs and sales tax.

| Product         | Supplier/Link                         | Cost   |
| --------------- | ------------------------------------- | ------ |
| Pack of wires   | https://www.adafruit.com/product/1957 | $1.95  |
| 1.8"LCD display | https://www.adafruit.com/product/358  | $19.95 |
| Total           |                                       | $21.90 |
