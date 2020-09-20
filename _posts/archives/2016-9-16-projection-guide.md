---
layout: post
title: Projection Guide
author: Hunter Korgel, August 2016
permalink: /video/projection-guide.html
---

# Video Rack and Projection System User Guide

## System Boot

First, make sure the MacPro is on and turn on the Projection System using the AMX controller at FOH (it will take a while for the lamp to warm up). Then, turn on the KUMO video switcher by flipping the KUMO’s power switch on the video rack under the FOH desk. Once the Projection System is live, use the AMX controller to set the Source to DVI 2, press ‘GO LIVE’, and unmute video (top left button).  

## MacPro Control System

Open Chrome on the MacPro and use the Bookmarks to open the Projector and KUMO controller pages in two separate tabs. The Projector page allows you to turn the lamp on and off and align, size, and focus the projected images. Do not mess with other settings on this page, such as the Title List. The Projector page is usually only used for setup and can be closed once you are done focusing. The KUMO page is where you will route all video sources and destinations, and should be left up throughout the duration of the show. To send a video source to a destination, first select the desired destination, then click on the input source you want to pull from. For example, to send the FOH HDMI feed to the stage patch, click output V37 Stg In to select the destination and then click input FOH HDMI to pull the input.  

## Focusing

You should focus the image as soon as you can, before you start working with content. Wait to focus until all soft goods are set if you’re using the scrim since you will have to work around legs, borders, etc. Similarly, don’t set the masking position until you have focused the image on the projection screen. Remember to keep the center speaker out of the projector’s path. You can use the following website for general focusing: http://www.aaarpinball.com/Miscellaneous/p1080.htm (I use Green Pluses and click the pattern for a fullscreen display).  

Sizing to the projection screen is simple: set the image to fit perfectly between the top edge of the white projection surface and the bottom edge of the roll. Avoid spillover by scaling the image smaller than the screen and slowly scaling it up to reach the top/bottom edges since it can be hard to notice the image on the black screen or hitting the stage below the screen’s roll. If the event is using the scrim for projection, placement and scale of the projection image depends on the specific needs of the group. Will there be dancers or musicians far upstage that could potentially block the image? Consult with the directors to get an image they are happy with that will be visible from almost all of the seats in the audience (someone sitting in the far left side of the house might not be able to see the left edge of the image if legs are in the way). Finally, make sure that the image is centered relative to masking, legs, or the center of the stage.  

Once the screen is scaled and placed properly, focus the image by looking at sharp edges and high contrast areas and sweeping along the zoom tool to find the optimal focus distance. It helps to switch between a focus image, high resolution images with moderate contrast (pictures of faces are good), and text.  

## Line Arrays and Surround Sound

When you turn on the Projection System, you also turn on the cinema audio system which includes the line arrays and the surround sound speakers around the hall. On most people’s presets they are controlled as a set of matrices which pick off sound sent to the mains, but you can set them up how you like. The line arrays must be flown in from the ceiling and are usually only used with the projection screen (it is ill-advised to send stage mics through the line arrays as you will have to fight a lot of feedback). The surrounds are set up as a stereo output (we do not have control over individual speakers like a 5.1 or 7.1 system). If you do use the surrounds in conjunction with the main speakers, make sure the surrounds are set to the correct delay time so that the audience doesn’t hear an echo from the two speaker systems.  

## Video Rack

The Video Rack is designed to be a black box, with users only having to understand what goes into it and what comes out of it. Normal use of the Video Rack does not require any changes to the individual components housed within, and users should aim to avoid diving into the rack by themselves. Keep in mind that the harder it is to get to a particular component, the less likely it is that you should be trying to get to it.  

![Video Rack Flowchart](/assets/video/projection-guide/video-rack-flowchart.jpg)

**KUMO Router**  
The KUMO is a 4out/16in video switching device that we use to manage all of our video routing within the performance hall. The outputs are the Projector, Preview Monitor, Crestron System, and Stage Patch V38. The inputs we use are the MacPro, FOH HDMI, Blu-Ray Player, Crestron System, and Stage Patch V37. The KUMO is controlled completely via the Chrome controller (described above) and the hardware in the rack is simply a hub of connection paths, so you should never have to change any of the connections in the rack.  

**Decimator**  
Within the Video Rack is a Decimator DMON-6S multi-viewer. This picks off video signals from each input and maps them to a 6 window multi-view display on the Preview Monitor without any required mapping from the KUMO. It also passes through each signal to the KUMO and stays on at all times. This does not require any attention for regular use as it stays on at all times (powered via power strip at bottom of rack(???)) and will never interrupt input signals to the KUMO. This device is connected to the MacPro via USB.  

**Converters**  
There are several video signal converters within the video rack, most of which are AJA HA-5 HDMI-HD SDI video/audio converters. Since most of our input sources and output destinations send and receive HDMI video signal, these converters surround the KUMO (which uses SDI for fast switching). The AJA converters are connected to the MacPro via USB, while other adapters such as the HDCP decoder for the in-rack Blu-Ray player are not connected. These converters are powered via the power strip located at the bottom of the video rack.  

**USB Hub**  
The USB Hub that connects the AJA converters and the DMON-6S to the MacPro is attached to the side of the wall on the back of the video rack. If you find that you cannot communicate with these devices, check the USB connections from this hub.  

**Stage Patch Points**  
Two SDI patches connect the stage patch and the KUMO video router: V37 input and V38 output. These connections are made under the FOH desk. In the amp room at the center stack, you can patch video signals to and from the AVPs around the stage to set up confidence monitors, take video feed from laptops on lecterns or backstage, or anything else you might need to do.  

## Projection Booth

The projection booth has more control surfaces for interfacing with the projector. The slide-out laptop can be used to save focus settings for shows that have multiple days of rehearsal or performance. You can also use built in high resolution focus and color spread test images to set your focus.  

## Troubleshooting

**My input isn’t showing up on the Preview Monitor!**  
First, make certain there are no problems with the input source. If there are no problems with the source itself, there is likely a loose connection at the AJA converter for your input. The AJA converters are located at the back of the video rack and are labeled according to the input or output they serve. On the side of the device are two lights that should be lit while functioning properly: a green light labeled POWER and an amber light labeled SDI LOCK. If either of these are off, check that all cables are plugged in and secure, and unplug and replug them all if necessary.  

**My stage patch isn’t working properly!**  
Confirm that the video rack V37 input and V38 output (these are both at the bottom of the back of the video rack) are connected to the V37 and V38 patch points under the FOH desk. Next, check the patch in the amp room’s center stack. If you are pulling video from a laptop on stage or backstage check that the AVP patch matches what you pulled from in the amp room. If you are having problems with a confidence monitor, refer to the confidence monitor guide after checking all patches.  

**I can’t get audio from my video input!**  
The Venue gets audio from the KUMO as a stereo AES(???) feed from the back of the video rack at the bottom. The video source should be set so that audio is sent through the video feed. For example, a MacBook on stage should have proper display settings and the audio settings should send out HDMI rather than speakers or headphones.

**The Projector is on, but it won’t display Program!**  
Go to the AMX controller at FOH and make sure that ‘Source’ is set to ‘DVI 2’, hit ‘GO LIVE’, and unmute the display. If it still isn’t working, go to the back of the video rack and find the AJA converter labeled ‘Projector’ and check all of the connections and indicator lights. Try unplugging all of the cables and plugging them back in. If it still isn’t working, go into the projection booth and check that the white DVI cable is plugged into (what is the port labeled?). If it still doesn’t work, turn the projection system off, then the KUMO, then the MacPro. Then turn on the MacPro, then the KUMO, then the projection system.
