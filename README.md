# Arduino FastLED Music Visualizer
An Arduino based music visualizer using the FastLED library and a strip of individually addressable LEDs.
<p align="center">
  <img width="200" height="300" src="https://github.com/the-red-team/Arduino-FastLED-Music-Visualizer/blob/master/images/mirrored_visualizer.gif">
</p>


# Table Of Constituents
- [Intro](#intro)
- [Setup](#setup)
  - [Materials](#materials)
  - [Standalone Arduino UNO Setup](#standalone-arduino-uno-setup)
  - [Arduino UNO with Sparkfun Spectrum Shield Setup](#arduino-uno-with-sparkfun-spectrum-shield-setup)

## Intro
Imagine this scenario. Does this not make you want to create your own music visualizer?

`> want to be super cool 1337 h4x0r 420 cuck`  
`> make led music visualizer from `[`the.red.team`](https://www.github.com/the-red-team)  
`> get it working perfectly`  
`> decide to use the shrooms my friend gave me for the first time and listen to music while watching the lights`  
`> nothing`  
`> nothing`  
`> need more shrooms but ate them all`  
`> leave house on scavenging mission in search of more fungal friends`  
`> crawled inside of the neighbor's dog`  
`> dog walks inside of neighbor house`  
`> broke into neighbor house by being inside of dog`  
`> it is night now`  
`> brown cow`  
`> creep upstairs to find their mushroom farm`  
`> go into bed room`  
`> nothing`  
`> turn to leave`  
`> emergency yogurt falls out of pocket onto hardwood floor of bedroom`  
`> yogurt everywhere`  
`> wife gets up`  
`> slips on yogurt`  
`> impaled by mattress and is dead`  
`> yogurt murder`  
`> heinous Crims`  
`> power dump on dad's face so he doesn't feel as bad about his dead yogurt wife`  
`> poop yogurt and leave`  
`> poo and yogurt all over`  
`> in the air`  
`> zero gravity and poop`  

I can't find a guide worth a shit on YouTube or Github. I saw many videos showing a demo of a DIY music visualizer using these exact lights and an arduino. People seem to love to brag about how awesome their shit is but they won't show you how to make it. I have created this repo for anyone who faces the same challenge I did. I hope you find this useful and beneficial to your daily intake of fiber.

# Setup
So this is how to setup the most "dank" music visualizer ever.  
There will be two ways to set this puppy up. I prefer the second way, but that costs money.

## Materials
- [Arduino UNO](https://www.amazon.com/gp/product/B01N4LP86I/ref=oh_aui_detailpage_o06_s00?ie=UTF8&psc=1)
- [WS2812b Individually Addressable LEDs](https://www.amazon.com/gp/product/B01CDTEJBG/ref=oh_aui_detailpage_o09_s00?ie=UTF8&psc=1)

## Standalone Arduino UNO Setup
### Pins
  - 5v - Connect to Vcc on LED strip
  - GND - Connect to GND on LED strip
  - A0 - Connect to the other end of the 3.5mm jack connected to your music source
    - A0 must be pulled down with a resistor (shown in the picture below)
  - 6 - Connect to DATA on LED strip
![alt text](https://github.com/the-red-team/Arduino-FastLED-Music-Visualizer/blob/master/images/circuit.JPG "Circuit")

## Arduino UNO with Sparkfun Spectrum Shield Setup
For this version of the music visualizer, you will need the [Sparkfun Spectrum Shield](https://www.amazon.com/gp/product/B00X0K30I6/ref=oh_aui_detailpage_o07_s00?ie=UTF8&psc=1)  
I prefer this version because it allows you to split the audio signal into 7 seperate channels (bass, mids, treb). This is important for anyone who wants their music visualizer to respond only to bass like mine. The sparkfun spectrum shield is...a shield...so you can solder the stacking female/male header pins to it and attach it to your Arduino UNO.
