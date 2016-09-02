---
layout: post
title: Video Overflow Setup
permalink: /video/overflow-video-streams.html
---
# Setting up Mezzanine and Lobby Overflow Video Streams

## Equipment

To set up a video feed for the Gidwitz Lobby Displays and the Mezzanine,
you will need the following equipment.

* (2) Decimator
* (3) SDI Cable
* (2) XLR Cable
* (3) HDMI Cable
* (1) XLR->RCA Cable
* (1) 1/4"->XLR Cable
* (1) Haivision Encoder (stays in the Amp rack)
* (1) Haivision Decoder (borrowed from another space)
* (1) Long (25ft or more) Ethernet Cable (will need to be checked out from the cage)
* (n) Large Portable TV (located on the 11th floor, will need to be checked out from the cage)
* (n) Hai-vision Decoder Remote

## FOH Setup

If there is an external videographer, skip this section. If there is no videographer, we will need to use equipment from the cage.
Check out a video camera and a tripod and set them up next to the FOH desk. We recommend the Sony PMW-EX1R HD Video Camera.

Set up an audio feed for the videographer's camera on the Venue with an AUX patched to an unused output(x).
This aux should include all live mics and digital audio channels.
Connect AUX-out(x) to the camera’s XLR-in and make sure the audio is routed to SDI-out on the camera.
Using the SDI cable, patch the camera into V40 at the FOH AVP under the desk.
Set up another AUX on the Venue (should be a copy of the first) so that it is patched to another unused output (y).

## Amp Room Setup

* Connect power to the Decimator.
* Patch V40 video output into Decimator SDI input using an SDI patch cable (these can be found on the wall and have a tube connection on one end and an SDI connection on the other).
* Connect the Decimator’s HDMI-out to the Haivision Encoder’s HDMI->DVI-in adapter using a short HDMI cable.
  * The encoder is located in the open slot in the rightmost rack towards the top, labeled 'Performance Hall'. You can place the Decimator in this slot next to the encoders.
  * To run the cable you will have to feed it through the opening and go around to the back of the rack with a flashlight to make the connection.
* Take output (y) you patched at the Venue from 'Venue Outputs' (center column in the amp room; APB-07; red and white labels) with ¼”->XLR cable, connect it to the XLR->RCA cable, and plug the RCA-outs into the RCA-ins at the back of the  encoder.
  * Again, feed the cable through the opening and go around to the back of the rack with a flashlight to make the connection.
* Run SDI from the Decimator’s SDI-out to SM console.

Decimator Settings: HDMI-out<-SDI-in, SDI-out(1)<-SDI-in (make loop)

## Stage Manager Console Setup
Set up a second Decimator with SDI-in taken from the Amp Room SDI run (on the floor, a shelf, or table is fine as long as the cables aren't a trip hazard).
Connect power to the Decimator, and send HDMI-out to Crestron panel’s HDMI-in using the second HDMI cable. Enter Technician Mode at Crestron panel (5540) and route “SM Input” to Lower Lobby, Auditorium, Theater East, and Theater West for overflow viewing.

Decimator Settings: HDMI-out<-SDI-in

## Theater East/West
Carefully remove the Decoder box from below the TV in either Theater West or Theater East. Make sure the disconnected cables are stable and accessible for reconnection during strike.
(When restoring these, take care with cable/port matches: Yellow Component cable -> Yellow Component output, Black/Silver Audio cable -> Red audio output)

## Mezzanine
* Connect the ethernet cable to left port (the right port is disconnected) of ethernet \#243 (located in the office to the right when you walk in) and connect the other end to “Primary” on the Decoder box.
* Plug in power for the TV, and plug the DC-Adapter into an outlet and connect it to the Decoder box.
* Run Component-outs from the Decoder to Component-ins on back of TV.
* Turn on TV and set to Component source.
* Run HDMI-out from the Decoder to HDMI-in on back of TV using the third HDMI cable.
* The following must be done quickly using the decoder remote:
  * select 1080i-out on Decoder
  * switch TV source to HDMI
  * hit accept/confirm on Decoder remote
