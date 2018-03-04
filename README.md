# AquaControl
Aquarium controller based on the Arduino Mega platform with TFT Touch and a relay system (Source code &amp; parts lists)

## About the project

This project is inspired by iAqua (or https://github.com/NineteenFire/MrAqua) and Robo-Tank (robo-tank.ca) and will control (almost) everything in my aqaruium with support for remote control and (maybe) be able to link with a smaller system (I.E an ESP8266 and DS18B20 temperature sensor) to show information from any other tanks (I.E hospital tanks) over a network connection

## Features

With some extra features I can't use yet.

- AutoPilot (make adjustments to the tank automatically based on some pre-defined options)

- Control of a relay board in a box (over a single CAT5E cable for referencing the relays to ground)

- Control of lighting in the tank (My tank doesn't have any fancy colour adjustment or fading, just two light tubes (white and blue))

- Temperature monitoring (DS18B20)

- pH monitoring - With it's ADC

- Lighting schedules

- Feeding/tank maintenance modes

- Fish intro mode (Not final, but it will disable bubblers/powerheads and slowly turn the lighting back on to introduce a new fish)

- Ability to add dosing pumps (I currently don't use them, but probably a good idea to add)

- Real time keeping (for AutoPilot)

- Remote control - Adjust AutoPilot settings & view values from sensors

- ATO (Auto top off) - My tank doesn't have this, but it will probably just be an option for one of the relays. (It fills the tank when 
it's a missing some water.)

- Filter, Heater, Powerhead, Bubbler & autofeeding support.

## Hardware

> Note: be careful buying very cheap hardware from eBay (especially the high voltage kit) not only is it a danger to your fish, but yourself.

- Arduino Mega (I'm personally using a geniune one, only for reliablility - you may want to use watchdog timer across the RST pin incase it crashes)

- 4 Channel Relay Board - I only have 4 things to control, but I will make the software support 16.

- DS16B20 Temperature Sensor - I don't have to explain what that's for (With it's pull-up resitor)

- Liquid PH0-14 pH sensor with BNC ADC - Monitor the pH of the tank along with it's ADC so the MCU can read from it.

- (Not Yet, later) Conductivity sensor - Oxygen sensor? - Water level sensor - Float switch

- 2x 2 Gang UK Sockets - So I don't have to cut the leads of any of my devices, just plug them in.

- 1x IEC Female connector - For connecting the relay box to a power supply easily.

- Some wood for making the enclosures for the relay box & controller/touchscreen.

- TFT Touch Screen (3.5") - Support may be added for the 2.4" TFT displays - With SD Card for logging & storing images.

- 10pcs 3Point THT screw down blocks (to easily connect the temperature sensor to the perfboard.)

- Perfboard (For making circuitry for some of the components - i.e a board with pull-up resistors to sensors)

- Solder & Tools

- A length of CAT5E cable (or some other form of cable, your choice, I just happen to have ALOT of CAT5E.)

- A length of cable for the high voltage side - In the UK I will be using 3 core electrical cable capable of 13Amps @ 230v (Keep to your countries regulations, don't mess with high voltage and don't get the cheapest thing you can find online.)

It looks alot worse written down like that, my system is at about £50.

## Credits

I will be using some code from other controllers & maybe some images, so I'll put a link to every project I copy code/assets from below with credit in the code and an OSS licenses page on the final project.

- 
