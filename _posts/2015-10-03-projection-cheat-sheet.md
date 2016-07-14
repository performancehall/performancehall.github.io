---
layout: post
title: Projection Cheat Sheet
permalink: /2015/10/03/projection-cheat-sheet.html
---

### BASIC

* SOURCE = MacMini or FOH HDMI

	1. Turn the Switcher Rack On (Black on / off flip switch, right side)
	2. On the AMX Touch interface, hit “Turn on system and projector"
	3. Open Chrome on the Mac Mini and Open the Kumo Bookmark
	4. Click Projector on the Bottom Row
	5. Select your source on the Top Row

![Image One](http://i.imgur.com/Hs68lLj.png)

##### If that doesn’t get you an image now we start:

<a name="troubleshooting"> *TROUBLESHOOTING* </a>

* Make sure you are actually sending some sort of image from your source: (very helpful to have the preview monitor at FOH set to the same source as the projector)
* If your source is the mac mini, try dragging a window to the right
* If you’re using a different source, make sure your display preferences are set up correctly
* Make sure the lamp of the projector is actually on
  * In Chrome, open the **Projector** bookmark. On the top left side there will be a little button that says Lamp and it will have on and off buttons on either side of the label. Make sure “ON” is selected.
* Make sure the image is not muted


![Image Two](http://i.imgur.com/xncCve2.png)


### INTERMEDIATE

#### SOURCE = STAGE

 AFTER YOU HAVE ALREADY DONE THE **BASIC** INSTRUCTIONS

 1. Get the Decimator, its power adaptor, and one of the long Blue SDI Cables* from Janice [When using the SDI cables, be gentle with them, be careful not to kink them, and please coil them properly when striking] . You may also need an extension cord and / or a power strip.
 2. Get whatever adaptors / other cables you need to be able send an HDMI signal to the Decimator from your source. (Probably a Thunderbolt to HDMI, or DVI to HDMI)
 3. Connect one end of the Blue SDI Cable to the SDI OUTPUT on the Decimator
 4. Connect the other end of the SDI Cable to one of the AVP Patch Points (If Downstage Right, use AV12, and run the cable up over the doorway.)
 4. Connect your source HDMI cable to the Decimator’s HDMI INPUT
 5. Confirm that your AVP Patch point (the one to which you connected the Blue SDI cable) is patched to AV38 in the patchbay (The default patching is AV12 to AV38)
 6. On the KUMO Routing Interface (Chrome), select Projector on the Bottom Row and STAGE on the Top Row.

That *should* get you an image. If it doesn't, refer to the [Troubleshooting](#troubleshooting) section above.

Then, if none of that works:

* Check Your SDI Patching.
* Check to make sure the Decimator is on (the screen will be lit).
* Check the BNC Patching in the Patchbay
* Check to make sure AV38 at FOH is actually connected to something, it should be SDI input #3 on the back of the AJA in the rack.

***

#### REFOCUSING / SIZING THE IMAGE (Basic/ Without Presets)

 1. Make sure the projector is on.
 2. Open the projector interface on chrome
 3. Click the “Basic Control” tab on the left
 4. Use the sets of arrows to adjust the image according to what you need

      *  For this you only have coarse adjust:
      * When you click an arrow it will continue to adjust in that direction until you click the square in the center of the arrows
	  * Also, when focusing, try and have someone on stage close to the screen (or whatever you’re projecting onto) to confirm the focusing

![Image Three](http://i.imgur.com/5Jrk0p3.png)

***

#### REFOCUSING / SIZING (Intermediate / With Presets)

You can do all the same things you can do from the web interface, and more, from the projection booth

1. Go into the projection booth
2. Check to make sure the computer is on
 * The computer is in the left rack, underneath the HDCam players, and underneath the screen that pulls out
 * It’s a 1U rack unit with a disk drive on the left and a “SuperLogics” logo, there is a red power button on the right.
 * Push the power button and the fan will start up, letting you know that it’s on.
3. Pull out the screen drawer (the black handle on the rack unit above the computer)
4. Click the **DCCs2** icon
5. In the communication settings window, make sure **Projector** is selected

 *  The IP Address is:  `192.168.1.134` Port is: `43728`

 ![Image Four](http://i.imgur.com/hx6h4VI.png)

6. Click OK (Also, the projector must be on in order to communicate with it. If it’s not on, nothing further will work. *And how were you planning to size an image if it’s off anyways?* :P

 ![Image Five](http://i.imgur.com/O1bGrL9.png)
7. Once the communication loading bar has completed and gone away, click the **lens** tab at the top.
8. From the lens tab you have access to the focusing and resizing adjustments, as well as Fine Adjust mode, and *presets*
	* SAVING A PRESET

 		* Make all the image adjustments you need
 		* Click the **Memory List** button to access the list of presets, then click a new row under all the ones that currently exist
 		* Click **Entry**, and name your preset, once it’s named you’re all good
 * LOADING A PRESET

 		* Select the preset you want to load
 		* Click the **Test** button, and the preset will begin to load

****

#### CONFIDENCE MONITORS

Using the Confidence Monitors is sort of the opposite of running a source from the stage in terms of signal flow.

1. Get out the Confidence Monitor rack case from Janice, grab one of the blue SDI cables, and get as many monitors and heavy duty DVI cables as you need.
2. Set up the case where it will live during the show, it needs power and needs to be relatively close to both an AVP, and the monitors to which you will be running the DVI cables.
3. Connect the power cord for the rack supply, and turn the rack on. There should be blue and green lights that indicate that the unit is on.
4. Connect the blue SDI cable to one of the AV patch points on the AVP
5. Make sure the patching in the patchbay is set up properly so that the AV patch point where you connected the SDI cable is hooked up to the point from where the signal at FOH is sending.
6. Connect the DVI cables from the back of the inside of the confidence monitor rack to the monitors you will be using, making sure to run the cable out of the way and to be gentle with the cable.

***
