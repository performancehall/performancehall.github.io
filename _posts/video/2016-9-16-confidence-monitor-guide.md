---
layout: post
title: Confidence Monitor Guide
author: Hunter Korgel, September 2016
permalink: /video/confidence-monitor-guide.html
---

# Confidence Monitor Guide

## One Confidence Monitor

**Equipment**  
(1) Decimator  
(1) 50’ SDI cable  
(1) short HDMI cable  
(1) Extension cord  
(1) Power Strip  
(1) Monitor (stored in Janice)  
(1) Monitor Power cable: Edison - IEC cable (usually with the monitor in Janice)  

**FOH Setup**  
Turn the video rack on and make sure the power strip on the bottom of the video rack is turned on as well. Open the KUMO controller (by opening chrome on the Mac Pro and clicking the KUMO bookmark) and set output ‘V38 Stg Out’ to pull from the input you are using for the monitor. Depending on what the speakers want, this could be a copy of what is displayed on the projection screen or presentation notes for a PowerPoint.

**Stage Setup**  
Set the monitor where the speakers want it, place the HDMI or DVI cable, Decimator and power strip under the lip of the stage relative to the monitor, and run the SDI cable from there to the nearest offstage AVP (the cable should run under the lip of the stage, up the side, and through the door to backstage). Run the extension cord in the same direction to pull power for the power strip. Plug in the Decimator and the power cable for the monitor, and connect the SDI cable to the Decimator’s SDI input. Plug one end of the HDMI cable into the Decimator’s HDMI output and the other end into the monitor. Dress cables and keep all of the non-monitor equipment under the lip of the stage and out of sight if possible.  

Decimator Settings: HDMI Out <- SDI In

**Amp Room Setup**  
Patch V38 to whichever port you used at the offstage AVP.

## Two Confidence Monitors

### **Doubled Display**

**Equipment**  
(2) Decimator  
(1) 50’ SDI cable  
(1) short SDI cable  
(2) short HDMI cable  
(2) Extension cord  
(2) Power Strip  
(2) Monitor (stored in Janice)  
(2) Monitor Power cable: Edison - IEC cable (usually with the monitor in Janice)  

**FOH Setup**  
Open the KUMO controller and set output ‘V38 Stg Out’ to pull from the input you are using for the monitor. Depending on what the speakers want, this could be a copy of what is displayed on the projection screen or presentation notes for a PowerPoint.

**Stage Setup**  
Set the monitors where the speakers want them and run the SDI cable from one monitor to the nearest offstage AVP (the cable should run under the lip of the stage, up the side, and through the door to backstage). Run the extension cord in the same direction to pull power for the power strip and set the strip under the lip of the stage. Plug in power for Decimator 1 and the power cable for the monitor, and connect the SDI cable to Decimator 1’s SDI input. Plug the HDMI cable into Decimator 1’s HDMI output and into the monitor. Dress cables and keep all of the non-monitor equipment under the lip of the stage and out of sight if possible.  

Decimator 1 Settings: HDMI Out <- SDI In, SDI Out (1) <- SDI In (make loop)  

Run the second extension cord from the first power strip to the second monitor and set up a power strip for the second monitor and Decimator 2. Connect the short SDI cable to Decimator 2’s SDI input and the second short HDMI cable to Decimator 2’s HDMI output. Again, dress cables and keep all non-monitor equipment under the lip of the stage and out of sight if possible.  

Decimator 2 Settings: HDMI Out <- SDI In  

**Amp Room Setup**
Patch V38 to whichever port you used at the offstage AVP.

### Independent Displays

**Equipment**  
(2) Decimator  
(2) 50’ SDI cable  
(1) short SDI cable  
(2) short HDMI cable  
(2) Extension cord  
(2) Power Strip  
(2) Monitor (stored in Janice)  
(2) Monitor Power cable: Edison - IEC cable (usually with the monitor in Janice)  

**FOH Setup**  
For two independent displays, we need to temporarily reconfigure the Video Rack. Familiarize yourself with the Video Rack first by reading through the Video Rack and Projection System Guide (I can put a link here when I build the page on the website). We want to hard patch a second stage output to the KUMO directly. (Are all of the outputs in fact used up???) Disconnect the output for the Crestron Video Rack (we need a number for this output, I think it is #3). Using the short SDI cable, connect the now open KUMO output to V39 on the FOH AVP under the desk. Open the KUMO controller and set output ‘V38 Stg Out’ to pull from the input you are using for the first monitor and set output ‘Crestron’ to pull from the input you are using for the second monitor. You can easily switch which monitor displays what in the amp room later, so don’t worry about that for now.  

**Stage Setup**  
Set the monitors where the speakers want them and run the SDI cables from the monitors to the nearest offstage AVPs (the cables should run under the lip of the stage, up the side, and through the door to backstage). Run the extension cords along the same respective paths to pull power for the power strips and set the strips under the lip of the stage. Plug in the Decimators and the power cables for the monitors, and connect the SDI cables to the Decimators’ respective SDI inputs and the HDMI cables to the respective Decimators’ HDMI outputs and into the monitors. Dress cables and keep all of the non-monitor equipment under the lip of the stage and out of sight if possible.  

Decimator Settings: HDMI Out <- SDI In  

**Amp Room Setup**  
Patch V38 and V39 to whichever ports you used at the offstage AVPs and check that the monitors are displaying the correct images for the speakers.  

## Three Confidence Monitors

Refer to the information under ‘Two Confidence Monitors’ to get the information you need for a three-monitor mixture of doubled displays and independent displays. We cannot support three independent displays for confidence monitors.
