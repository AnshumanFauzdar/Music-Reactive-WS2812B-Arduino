[![](https://img.shields.io/github/stars/AnshumanFauzdar/Music-Reactive-WS2812B-Arduino?style=for-the-badge)]()
# Music-Reactive-WS2812B
LED STRIP WS2812B reacting to music connected through your AUX 3.5mm Jack
Connections are simple and you can connect 2 LED strips - WS2812B and can change effects by pressing button [Push Button]

Arduino Mega is highly recommended as UNO is only capable of processing upto 50 LEDs more precisely upto 30 is processed
For 30+ LEDs use Mega instead of Uno

PS:- There are 2 versions of code in Folder "CODES" you can check both of them, which suits you Version 2.0 is stable and working smooth without any glitches

# Preparing Arduino Libraries

This step is very important as your arduino need some FAST LED and NEOPIXEL library to work upon for your WS2812Bs

Download FAST LED libraries from Github(link in description) or simply go to ---->Sketch/Include_Library/Manage_Libraries/ and search for FAST LED - FastLED by Daniel Garcia and install, do restart your IDE to take effect

Do search for NEOPIXEL "https://github.com/adafruit/Adafruit_NeoPixel" and install in same way as Procedure above

For other cool effects for your WS2812B you can add WS2812FX library "https://github.com/kitesurfer1404/WS2812FX" [Same way as for Fast LED] - Cool and funky features are added for WS2812Bs

Keep the Codes in one folder contaning other libraries --->rgb.h ---->rgb_operators.h ------>water_torture.h //Not doing so will give you compiling errors//

# Arduino Schematics and Connection

For complete wiring of WS2812B AKA Neopixel you should read complete detail on "https://learn.adafruit.com/adafruit-neopixel-uberguide/basic-connections" for power distribution and other details for which these WS2812B are sensitive to

Now coming to connection, always remember to attach common ground wiring, as not doing so can destroy you components!

For Aux connection coming from your phone, laptop or any other source......

Connection:

             Ground to Ground

            
             Black wire to Analogue Pin 4 - A4
             
             
             Red Wire to Analogue Pin 5 - A5
             
             
        //If ground is both in RCA cable, connect both - mostly AUX cables have 1 ground cable//
        
If connection of arduino and audio source is same that is if you are using your PC, then there is no need to connect GND of AUX to Arduino board        

Complete Schematic Diagram for connection guide:

![alt text](https://user-images.githubusercontent.com/40523329/42878038-497a6bbc-8aa9-11e8-8569-0bb6781f5f54.png)

This connection is for only one LED Strip and you can connect two LED strips to board on PIN 5 and 6 [Can adjust to your configurations]

And connect GND of PushButton [Any part of button] and other[other than GND] to input 0 PIN [RX written on PIN] on arduino board

# Final Conclusion

This project is in development phase, and lack some coding details and other parameters

In future, ESP8266 Wifi module will be added to this and will work like a project on IOT [Internet OF Things]

Currently all credits goes to "Cine Lights" for schematics and Arduino Code

# Errors and Issues

//PLEASE PUT ALL THE FILES OF "CODES" folder in one place to work without any error//

Code has been tested and works smooth, without any error [Version 2.0 is more smooth and better]

ARDUINO UNO - Sometimes after defined clicks of button, Board runs random programs [Means Crash] this is due to low memory of UNO, Arduino Mega is higly recommended

# CREDITS goes to Cine-lights for amazing code and work done

Subscribe to channel for all the work [Cine-Lights](https://www.youtube.com/channel/UCOG6Bi2kvpDa1c8gHWZI5CQ)
