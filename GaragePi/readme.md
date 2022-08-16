# Documentation for GaragePi Setup

## Background

I found this setup that was posted by [Renjith Nair](https://renjithn.com/garagepi-garage-opener-using-raspberry-pi/), but found the instructions listed either made assumptions on how to do something or have changed with newer releases of software.  Below are the steps I took to create my GaragePi and get it working with Home Assistant.  I also modified it to work my garage door opener lights.

A little additional background.  I have had a Garage_Pi setup for about 6 years using [Andrew Shillday's setup](https://github.com/andrewshilliday/garage-door-controller).  However, I broke it a while back while trying to better secure it and trying to add some additional functionality.  I didn't have the time or knowledge to get it working at that time, so it has sat for about 6 months while I was working on other things.  I recently setup Home Assistant, which got me thinking about the GaragePi again.  And that's where we are today.

I will not be going through the steps to do the initial setup of a Raspberry Pi as it is well documented on [raspberrypi.com](https://www.raspberrypi.com/software/) (installing and initial setup of Raspberry Pi OS).

## Components in my setup
- Raspberry Pi 3B running Raspberry OS (Bullseye at the time of this writing)
- A P/N 8601 Magnetic Switch for each Garage Door (2 in my case)
- Some low voltage wire (I used left over from garage door controller install)
- A 4 Channel 5V Relay Switch Module similar to [this one](https://www.amazon.com/JBtek-Channel-Module-Arduino-Raspberry/dp/B00KTEN3TM)
- A bread board to make things a little easier to connect (I will likely remove this at some point)
- A GPIO breakout similar to [this one](https://www.amazon.com/Adafruit-2028-Assembled-T-Cobbler-Plus/dp/B00OG4X0DK)
  - I will likely change this out to one of [these](https://www.amazon.com/Ultra-Small-Status-Terminal-Breakout-Raspberry/dp/B09QXR6RL7) at some point to clean it up a little.
- A mounting board (plastic) that I found somewhere years ago.  I will also likely redo this and design something to print (or find something to print) to hold the components to help with the WAF (Wife Acceptance Factor).
- Home Assistant
  - Below I will cover how I set this up on a Raspberry Pi and it's actually pretty much identical to installing Raspberry Pi OS.
  - I am using a Raspberry Pi 4 to run it, but it can be run on other OS's also.  Check out [home-assistant.io]https://www.home-assistant.io) for more information.
  - I am using a 64GB SD card for my Home Assistant.  I wanted to make sure to have a decent amount of storage for it.

## Setup Home Assistant

[homeassistant.md](./homeassistant.md)

## Raspberry Pi Configuration

1. 
