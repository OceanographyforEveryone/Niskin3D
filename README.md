Niskin3D
========

### Background

Niskin3D is low-cost, open-source water sampler made from 3D-printed parts and controlled by a waterproof servo. 

![](https://github.com/OceanographyforEveryone/Niskin3D/blob/master/Images/IMG_20190212_174718211.jpg)

### Overview

The Niskin bottle, a seemingly simple tube designed to take water samples at discrete depths, is one of the most important tools of oceanography. Coupled with a CTD, an array of Niskin bottles fit into a rosette provides everything an oceanographer needs to profile the ocean. Niskin bottles are neither cheap nor particularly easy to use. A commercial rosette requires a winch to launch and recover, requiring both a vessel and a crew to deploy. For informal, unaffiliated, or unfunded researchers, as well as citizen scientists or any researcher working on a tight budget, getting high-quality, discrete water samples is an ongoing challenge. 

The Niskin3D lowers the cost of discrete-depth water sampling and makes this common tool of oceanographic research available to anyone. 

### Current Status

Undergoing major redesign as of 2/12/2019.

### Bill of Materials

We use Amazon Affiliate links because the small kickback helps fund more projects like this, but almost everything can be sourced through hobby shops, hardware stores, and other retailers. These recommendations don't necessarily represent the cheapest prices but rather the actual components we bought for this project or the closest approximation we could find. Some components are batched and may be available elsewhere in smaller quantities. Other high-test line and elastics can be used in place of the monofilament and sligshot tubing. 

**Niskin3D Bottle and Trigger Mechanism**

Part | Supplier | Price | Link
--- | --- | --- | ---
HiTec 32646W HS-646WP Water Proof Analog Servo (IP-67 Rated) | Amazon | $44.36 | https://amzn.to/2E60NLb
Clear Polycarbonate Tubing, 1-1/8" ID, 1-1/4" OD, 1/16" Wall, 4' Length | Amazon | $11.72| https://amzn.to/2E66wRa
Solid Rubber Stoppers - Size 6 | Amazon or local hardware store | $10.88 | https://amzn.to/2E6pEyw
Eye Screw with 12mm hoop | Amazon or local hardware store | $6.89 | https://amzn.to/2U5frI4
150-lb Monofilament with 1.3mm Crimps | Amazon or local fishing store | $12.99 | https://amzn.to/2tmStAh
3x5mm Natural Latex Rubber Band Tube Tubing for Slingshots | Amazon or local sportiing good store | $7.55 | https://amzn.to/2GGn57R
8" Cable Ties | Amazon or local hardware store | $6.99 | https://amzn.to/2E7rf76

**Niskin3D Control Box**

Part | Supplier | Price | Link
--- | --- | --- | ---
Arduino Leonardo | Amazon or Arduino.org | $22.19 | https://amzn.to/2E66RDo
2K Ohm Potentiometer | Amazon | $13.21 | https://amzn.to/2SGJUil
Ribbon Cable | Amazon | $6.98 | https://amzn.to/2UPQDDK
M3 Hex Socket Screws | Amazon | $10.99 | https://amzn.to/2GnfeN8

Consumables include heat shrink tubing, solder, and hook-up wire. Tools include a crimper, flush cut pliers, hex wrench, and a soldering station. We recommend using PLA filament for the 3D-printable parts. 

### Build Instructions

**3D Printing.** Print all parts in [3D_Printer_Files](https://github.com/OceanographyforEveryone/Niskin3D/tree/master/3D_Printer_Files) (ignore the folder labelled old unless you want to build the original Niskin3D) using your prefered PLA filament. NiskinRecieverLinear.stl, PowerBox.stl, and PowerBoxBottom.stl should be printed at 200 micron resolution with 20% infill. All other components should be printed at 100 micro resolution with 100% infill. 

**Servo Assembly.** Remove the included servo horn and slot the servo wheel onto the exposed metal gear. Use the included screw to secure the wheel. 

![](https://github.com/OceanographyforEveryone/Niskin3D/blob/master/Images/IMG_20190212_145143.jpg)

**Receiver Assembly.** Insert the servo into the reciever such that when holding the reciever with the trigger tube facing away from you, the servo wheel sits to the right of the trigger slot. 

![](https://github.com/OceanographyforEveryone/Niskin3D/blob/master/Images/IMG_20190212_145200.jpg)

Rotate the servo wheel counter-clockwise until it reaches its limit. Slot the trigger through the external trigger hole and across the servo wheel and just barely into the main trigger slot. The innermost tooth of the trigger should fully catch against the servo wheel. Secure the trigger to the reciever by looping monofilament through the hole in the trigger and the loop near the base of the reciever to prevent the trigger from being lost if it comes loose.

![](https://github.com/OceanographyforEveryone/Niskin3D/blob/master/Images/IMG_20190212_145215.jpg)

**Bottle Assembly.** Cut the polcarbonate tube to the deisred length. Screw the eye screws into the center of both faces of the rubber stopper. Crimp monofilament onto the wider face of each stopper. On one stopper, measure out enough line to reach the hole in the center of the reciever trigger tube and crimp a large loop into the monofilament. On the other stopper, measure out enough line to  reach the hole in the center of the reciever trigger tube with enough length the the pin can sit in the center of the trigger tube and crimp the monofilament around the pin with enough slack that the line can sit in the notch on the pin. 

![](https://github.com/OceanographyforEveryone/Niskin3D/blob/master/Images/IMG_20190212_145313.jpg)

Measure out enough latex tubing that it can hold the two rubber stoppers tightly in the polycarbonate tube. On the inner face of one rubber stopper, ziptie the latex tubing to the eye bolt. Feed the latex tubing through the polycarbonate tube, pull it tight, and ziptie it to the inner eye bolt on the other rubber stopper. 

**Power Box Assembly.** _Only do this if you need an independently-triggered Niskin bottle. Otherwise, connect the servo to the hardware of your choice using a standard servo interface._  Flash [NiskinServo.ino](https://github.com/OceanographyforEveryone/Niskin3D/tree/master/NiskinServo) to the Arduino. Solder header wires to the potentiometer. Screw the potentiometer into the large hole in the center of the Power Box Bottom. Connect the outer leads of the potentiometer to ground and Vin. Connect the center lead to Analog Pin 0. Measure out as much ribbon cable as you need for the servo. Feed ribbon cable through hole next to the spool on the case. Connect servo to ground and 5V. Connect signal line to Digital Pin 7. Close case and secure with M3 screws.

![](https://github.com/OceanographyforEveryone/Niskin3D/blob/master/Images/IMG_20190212_145938.jpg)

### Priming the trigger

Pull the rubber stoppers out of the polycarbonate tube. Slot the pin into the trigger tube such that the point sticks up through the central hole. Rotate the servo clockwise to drive the trigger through the pin and into the wall of the trigger tube. Slot the loop on the other stopper through the trigger tube and over the pin such that it catches and rotates the pin towards the opposite rubber stopper. 

![](https://github.com/OceanographyforEveryone/Niskin3D/blob/master/Images/IMG_20190212_175831.jpg)

Ensure that the rubber stoppers are situated so that once the pin is released both stoppers will be pulled into the polycarbonate tube and seal it. 

Your Niskin bottle is now primed. 

### Triggering

Activate the servo and rotate it counter-clockwise to pull the trigger and release the pin. 

### Resources and Media

[Oceanography for Everyone](http://oceanographyforeveryone.com/)

[Niskin3D: the open-source water sampler](https://www.thingiverse.com/thing:3421202)

[A 3D-printable, drone and ROV-mountable, water sampler](http://www.southernfriedscience.com/?p=18730)

[The next generation open-source, 3D-printable Niskin bottle has arrived!](http://www.southernfriedscience.com/the-next-generation-open-source-3d-printable-niskin-bottle-has-arrived/)

### Acknowledgments 

Design and testing of the Niskin3D conducted by Andrew Thaler.

### Code of Conduct

Please review our [Contributor Code of Conduct](https://github.com/OceanographyforEveryone/Niskin3D/blob/master/CODE_OF_CONDUCT.md) prior to your first contribution. 
