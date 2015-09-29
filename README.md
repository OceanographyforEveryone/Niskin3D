Niskin3D
========

[Link](http://www.southernfriedscience.com/?p=18730): Southern Fried Science Project Description

###Background

Niskin3D is low-cost, open-source water sampler made primarily from 3D printed parts and controlled by a simple servo. 

###Overview

The Niskin bottle, a seemingly simple tube designed to take water samples at discrete depths, is one of the most important tools of oceanography. Coupled with a CTD, an array of Niskin bottles fit into a rosette provides everything an oceanographer needs to profile the ocean. Niskin bottles are neither cheap nor particularly easy to use. A commercial rosette requires a decent-sized winch to launch and recover, which means you need a vessel and a crew to deploy. For Rogue Ecologist and citizen scientists, getting a high-quality, discrete water sample is a perpetual challenge. With tools like the OpenROV and the soon-to-be-completed EcoDrone, we wanted a Niskin bottle that was light weight and capable of being mounted on both underwater robots and quadcopters with ease.

###Bill of Materials

Almost all of the necessary parts can be found through Amazon. Visit our [Parts Depot](http://oceanographyforeveryone.com/depot.html) for the full list. 

The Niskin3D uses the [OpenROV prototype underwater servo](http://store.openrov.com/collections/experimental/products/prototype-underwater-servo), though any other waterproof servo will also work, provided you adjust the size of the servo basket on the reciever. 

###Build Instructions

Print out all the parts. If you want to mount the bottle to the payload bay of an OpenROV, print the NiskinOpenROVClip.stl file. While everything is printing, screw the crown bolts into the rubber stoppers, on both ends. Cut the polycarbonate tube to desired length, debur, and chamfer the inner edges to prevent the stoppers from catching.

Insert the servo into the trigger receiver such that the wires line up with the slot and hole. Mount the receiver to the center of the tube with zipties. Mount the end catches to the edges of the tube, making sure that they’re inline with the receiver. Tie off the elastic to one stopper and feed it through the tube. Tie off the elastic to the other stopper such that there’s enough tension to snap tight. Measure out enough fishing line that the stoppers are held open when the line is pulled to the center of the tube.

Here’s the trick bit. One side of the receiver has a groove that allows the wire from the servo to slide in. Tie the pin to the rubber stopper on the non-wire-side of the receiver, there’s a small notch that indicates where the pin should be tied. Tie a big loop in the other line. Mount the trigger underneath the plastic arm of the servo with a paperclip. Lock the servo arm in place such that when fully extended trigger-side, the trigger rests tightly in the vertical slot in the middle of the receiver. You may have to power on the servo to determine where the fully extended position is. Wire up the servo to your control unit of choice. Walt Holm has some excellent advice for connecting to an OpenROV control board.

If you’re mounting to an OpenROV, mount the OpenROV clip to the front two bars of the payload bay and zip tie the bottle underneath.

###Priming the trigger

Pull the pin-side rubber stopper up through the catch as shown. Slide the pin into the receiver and rotate until the post comes up through the center hole. Rotate the trigger into place. Pull the rubber stopper off the catch and place it in the open position. The pin should lock in place. Now open the other stopper, slide the loop through the receiver slot, and loop it over the post on the pin. The pin will catch, rotate, and lock against the opposite side of the center hole. This positioning ensures that when the trigger is released, both end will be freed simultaneously.

###Triggering

Using your controller of choice, activate the servo. Both stoppers should slam shut as soon as the trigger clears the pin.

###Resources
[Oceanography for Everyone](http://oceanographyforeveryone.com/)

[Original Project Description](http://www.southernfriedscience.com/?p=18730)

###Acknowledgments 

Design and testing of the Niskin3D conducted by Andrew Thaler.
