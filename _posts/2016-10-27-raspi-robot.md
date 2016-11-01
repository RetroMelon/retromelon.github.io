---
title: Browser Controlled RPi Robot w/ Live Video and Speech Synthesis
updated: 2016-10-27 15:56
type: project #making the type project will pull this into a different category.
featured: 1
---
<iframe class="youtube" src="https://www.youtube.com/embed/F3hmwtnsWZA" frameborder="0" allowfullscreen></iframe>

Above is a quick (2:50 minute) video about my Raspberry Pi robot. I built this as an experiment and to test my skills interfacing a digital raspberry pi with some (very basic) analog DC motors. I also thought the idea of a physical device was quite fascinating and exciting!

The robot server runs on node.js which accepts commands from the web interface via websockets. It uses some of the RPi GPIO pins to transmit PWM signals to an L298D motor controller, which in turn controls the DC motors.

This project was inspired by [Shaunuk](https://github.com/shaunuk)'s similar project using a converted RC car.

### Getting your hands on the code

> All of the code for this robot is on github: [**here**](https://github.com/RetroMelon/Raspberry-Pi-Car).

Some tweaking of output pins and wifi configurations might be necessary to get this running on your own hardware.
