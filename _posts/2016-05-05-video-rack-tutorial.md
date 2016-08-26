-
  layout: post
  title: Video Rack Guide
-

## Intro

The video rack is a bit of a beast of a rig. Don't be frightened by it.
There are a lot of wires and components on the inside of it, but most of the actual signal flow is relatively simple. In this tutorial we'll break down the sections of it that you need to know, and explain how the signals flow into, out of and within the rack. 

## Major Sections

Mac Pro
Multiview
Converters
IO Panel
USB Hub

## IO Panel

This is where all the signals come into and out of the rack. As such, if you need to troubleshoot anything, this is the place to start. In an ideal world, you shouldn't change anything further down the signal chain than the IO Panel. If changing things here doesn't resolve your issues, think long and hard before you go changing any connections beyond this point.

#### IO Panel Connections

* SWITCHED:
  
  This is the switched power that feeds the Furman relay. It is switched via the switch on the front of the Furman, and feeds power to a number of the video converters.
  
* UNSWITCHED:

    * This power connection feeds :
    
* Creston:
  
  * This is the Crestron Fiber optic connection 

* FW32
* NETWORK
* NETWORK

* USB

* PROJECTOR:

    * This is the DVI feed out to the Projector. The cable travels along the trough under FOH and comes up in Projection Boot and plugs into one of the DVI ports on the bottom of front panel of the left most rack by the projectors. 
    
* STAGE IN SDI
    * This is fed from V37 and is used to route a signal from somewhere on stage up to the KUMO
* STAGE OUT SDI
    * This feeds V38 and is used to route a signal from one of the KUMO inputs to a display feed somewhere other than FOH, usually for confidence monitors or projectors on stage. 
* AMX MON 
    * (INACTIVE?)
* BLANK SDI
  
* FOH IN
    * This is where the FOH HDMI cable patches into the video rack. From here it connects to the FOH HDMI AJA Converter and from there into the Decimator Multiview and on to the KUMO.
* MULTIVIEW
    * This is the HDMI feed that comes from the Multiview and goes to the Right hand Display on the FOH desk.
* DISPLAY (?)
* CRESTRON
    * This is the HDMI port that feeds the HDMI input on the Crestron panel on the ABP under the FOH Desk. 

MIDI IN
MIDI OUT
* AES3 IN
* AES3 OUT
* KUMO L
* KUMO R

### Making Sense of it All

The biggest thing that will help you to understand how the video rack works is to have an understanding of the underlying signal flow. If you can understand how the signals move around and are altered in an abstract fashion, making sense of the cable mess becomes, if not easier, then a little more straightforward. 

The video signals that run into, out of and around the video rack come in two 'flavors', SDI (specifically ________) and HDMI. Any time you need to make a change between the two formats, you need a converter. The converters in the rack take the form of the small grey AJA boxes. These AJA boxes accomplish the same function as the larger, bright red Decimator boxes that you may have seen around before. 

Now, why exactly are we converting between SDI and HDMI in the first place? Why can't we just use one format? The answer to those questions has to do with the nature of the Hardware we use for various purposes in the hall. HDMI can be thought of as more of a consumer level format. You use it to connect your laptop or computer to a monitor or TV or a small projector. SDI on the other hand, is a format used in higher profile professional hardware, such as the NEC Projector (the one in the projection booth), video switching hardware like the AJA KUMO, and for transporting video signals over distances longer than a couple feet without signal degradation. 

Since we often deal with multiple video signals that we like to be able to switch between for displaying various media during shows, we use specialized hardware to be able to switch between all of our signals. For us, this hardware is the AJA KUMO 1604, which has 16 SDI inputs and 4 SDI outputs. The KUMO can route any of the 16 inputs to any of the 4 outputs and can switch back and forth relatively seamlessly, with control being accessed via a network connection than you can call up in a browser (See the 'KUMO' bookmark in Chrome on the FOH Mac Pro). 

So if we have an HDMI signal on a laptop at FOH that we want to be able to route to a display on stage, one way to do this would be to just hook the HDMI up to a Decimator, take the SDI output, patch it to the ABP and do the opposite on stage. However if we want to be able to switch the signal that the display receives, we would want to hook the HDMI upto an HDMI to SDI converter (like the Decimator or the AJA boxes), and run the SDI into the AJA, so that we can switch the display's feed back and forth between this HDMI and the other signal. 

#### Multiview

So we've covered why we need to convert signals and how the KUMO accomplishes the signal switching we like to be able to do, but one thing we've yet to discuss is the Multiview and how that fits into the signal chain. 

When we're switching back and forth between the various video feeds we have to deal with during a show, it's convenient if not necessary to be able to see what each signal is to ensure that we're not going to go live on a blank screen or some other unsuitable feed. The Multiview allows us to quickly inspect a lot of different signals quickly to make sure everything is how it should be. However in order to do this, it needs all the signals we worry about to flow through it. This makes our lives a little more difficult in terms of troubleshooting things, and certainly makes the video rack a lot messier, but provides necessary functionality that outweighs these costs. 

So to revisit our previous example, we have an HDMI signal we want to be able to get from a laptop at FOH down to a display or projector on the stage. We patch into the FOH HDMI cable that sits at the desk. That cable goes into the IO Panel on the back of the video rack. From there an HDMI cable runs inside the rack to an AJA HDMI to SDI converter. The SDI cable that comes out of that carrying our signal goes into an input on the multiview and comes out unchanged on a loop output from the multiview. From the multiview the new SDI cable patches to an input on the back of the AJA KUMO. 

An important part of this is that the signal the Multiview is getting and showing us from the FOH HDMI is the same as the signal it then sends to the input on the KUMO. The multiview lets us look at a number of the signals we're getting on the 'Preview Monitor', so that we can know what we're getting before we switch our signals with the KUMO. 

