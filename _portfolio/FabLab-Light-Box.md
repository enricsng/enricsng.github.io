---
title: "Light Box Game"
excerpt: "I created a game using an arduino. <br/><img src='/images/box-light.jpg'>"
collection: portfolio
date: 2024-02-01
---

![Light Box Game](/images/box-light.jpg)

# Task
As part of the SUTD open house event, I was asked to create a display at the Fabrication Lab on campus. I decided to create a light box game that would engage visitors and showcase the capabilities of the lab.

The light box was made using acrylic sheets and MDF, given that I had prior experience in using these materials.

# Physical Design
The light box consisted of a MDF frame with a transparent acrylic sheet on top. Inside the box, I placed an LED strip that could be controlled using an Arduino. These designs were designed in Fusion 360, and cut using a vertical saw and scroll saw.
![Box Side View](/images/box-side.jpg)

# Electrical Design
WS2812B LEDs were used for the light box. These LEDs are individually addressable, allowing for a wide range of lighting effects. The LEDs were controlled using an Arduino Mega, which was programmed using the FastLED library. The Arduino was powered using a 5V power supply.

However, since the spacing of the leds was too short, I needed to extend the length. I meticulously soldered the wires to extend the length of the LED strip. Doing all 16 leds took quite a long time, because each diode had 3 wires.
![Box Electrical](/images/box-electrical.jpg)

On top of that, I had to get the sensors working to detect the movement of the users. I used a IR sensor to detect the movement of the users. The sensor was connected to the Arduino, and the Arduino would change the lighting effects based on the sensor input. The IR was able to pass through the acrylic sheet, but the user could not see it.
![Box Sensor](/images/box-sensor.jpg)