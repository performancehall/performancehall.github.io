---
layout: post
title: Video Overflow Setup
permalink: /2016/03/08/overflow-video-streams.html
---
# Setting up Mezzanine and Lobby Overflow Video Streams

## Equipment

To set up a video feed for the Gidwitz Lobby Displays and the Mezzanine,
you will need the following equipment.

* (2) Decimator
* (3) SDI Cable
* (2) XLR Cable
* (2) HDMI Cable
* (1) XLR->RCA Cable
* (1) 1/4"->XLR Cable
* (1) Long Ethernet Cable (will need to be checked out from the cage)
* (n) Large Portable TV (11th floor)
* (n) Decoder Remote

## FOH Setup

Set up an audio feed for the camera on the Venue with an AUX patched to an unused output(x).
Connect AUX-out(x) to  camera’s XLR-in and make sure the audio is routed to SDI-out on the camera.
Using the SDI cable, patch the camera into V40 at the FOH AVP under the desk.
Set up another AUX on the Venue (should be a copy of the first) so that it is patched to another unused output (y).

## Amp Room Setup

* Connect power to the Decimator.
* Patch V40 video output into Decimator SDI input.
* Connect the Decimator’s HDMI-out to the Encoder’s HDMI->DVI-in adapter.
  * The encoder is located in the open slot in the rightmost rack towards the top, labeled 'Performance Hall'.
* To run the cable you will have to feed it through the opening and go around to the back of the rack with a flashlight to make the connection.
* Take output(y) you patched at the Venue from 'Venue Outputs' (center column in the amp room; APB-07; red and white labels) with ¼”->XLR cable, connect it to the XLR->RCA cable, and plug the RCA-outs into the RCA-ins at the back of the  encoder.
* Run SDI from the Decimator’s SDI-out to SM console.

Decimator Settings: HDMI-out<-SDI-in, SDI-out(1)<-SDI-in (make loop)

## Stage Manager Console Setup
Set up a second Decimator with SDI-in taken from the Amp Room SDI run.
Connect power to the Decimator, and send HDMI-out to Crestron panel’s HDMI-in. Enter Technician Mode at Crestron panel (5540) and route “SM Input” to all the TVs you want to use for overflow viewing.

Decimator Settings: HDMI-out<-SDI-in

## Theater East/West
Remove the Decoder box from below the TV in either Theater West or Theater East.
(When restoring these, take care with cable/port matches: Yellow Component cable -> Yellow Component output, Black/Silver Audio cable -> Red audio output)

## Mezzanine
* Connect the ethernet cable to left port under Erin's desk (the right port is disconnected) and connect the other end to “Primary” on the Decoder box.
* Plug in power for the TV, and plug the DC-Adapter into an outlet and connect it to the Decoder box.
* Run Component-outs from the Decoder to Component-ins on back of TV.
* Turn on TV and set to Component source.
* Run HDMI-out from the Decoder to HDMI-in on back of TV.
* The following must be done quickly using the decoder remote:
  * select 1080i-out on Decoder
  * switch TV source to HDMI
  * hit accept/confirm on Decoder remote
