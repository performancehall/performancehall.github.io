---
layout: post
title: Projection Cheat Sheet
permalink: /2016/8/28/projection-cheat-sheet.html
---

###BASIC

* SOURCE = Mac Pro or FOH HDMI

	1. Turn the Switcher Rack On (Black on / off flip switch, right side)
	2. Make sure the Roland video switcher powers on
	3. On the AMX Touch interface, hit “Turn on system and projector"
	4. Wait for the projection system to finish booting
	5. On the Roland Video Switcher, press the top row button that matches your source. It should light up red.

#####If that doesn’t get you an image now we start:

<a name="troubleshooting"> *TROUBLESHOOTING* </a>

* Make sure you are actually sending some sort of image from your source: (very helpful to check the preview monitor at FOH - every source will be displayed)
* If your source is the Mac Pro, try dragging a window to the right
* If you’re using a laptop or other external source, make sure your display preferences are set up correctly
* Make sure the lamp of the projector is actually on
  * In Chrome, open the **Projector** bookmark. On the top left side there will be a little button that says Lamp and it will have on and off buttons on either side of the label. Make sure “ON” is selected.
* Make sure the image is not muted


![Image Two](http://i.imgur.com/xncCve2.png)


###INTERMEDIATE

####SOURCE = STAGE Input V37

 AFTER YOU HAVE ALREADY DONE THE **BASIC** INSTRUCTIONS

 1. Get the Decimator, its power adaptor, and one of the long Blue SDI Cables* from Janice [When using the SDI cables, be gentle with them, be careful not to kink them, and please coil them properly when striking] . You may also need an extension cord and / or a power strip.
 2. Get whatever adaptors / other cables you need to be able send an HDMI signal to the Decimator from your source. (Probably a Thunderbolt to HDMI, or USB-C to HDMI)
 3. Connect one end of the Blue SDI Cable to the SDI OUTPUT on the Decimator
 4. Connect the other end of the SDI Cable to one of the AVP Patch Points
 5. Connect your source HDMI cable to the Decimator’s HDMI INPUT
 6. Confirm that your AVP Patch point (the one to which you connected the Blue SDI cable) is patched to V37 in the patchbay
 7. On the Roland Video Switcher's top row, select V37. It should light up red.

That *should* get you an image. If it doesn't, refer to the [Troubleshooting](#troubleshooting) section above.
section above.

Then, if none of that works:

* Check Your SDI Patching.
* Check to make sure the Decimator is on (the screen will be lit) and configured properly. Refer to the Decimator Operator Manual if needed.
* Check the BNC Patching in the Patchbay
* Check to make sure V37 at FOH is connected to Input 1 on the Roland Video Switcher.

***

####REFOCUSING / SIZING THE IMAGE (Basic/ Without Presets)

 1. Make sure the projector is on.
 2. Open the projector interface on chrome
 3. Click the “Basic Control” tab on the left
 4. Use the sets of arrows to adjust the image according to what you need

      *  For this you only have coarse adjust:
      * When you click an arrow it will continue to adjust in that direction until you click the square in the center of the arrows
	  * Also, when focusing, try and have someone on stage close to the screen (or whatever you’re projecting onto) to confirm the focusing

![Image Three](http://i.imgur.com/5Jrk0p3.png)

***

####REFOCUSING / SIZING (Intermediate / With Presets)

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

####CONFIDENCE MONITORS

Using the Confidence Monitors is sort of the opposite of running a source from the stage in terms of signal flow. While V37 connects to the Roland Video Switcher, the Kumo houses a secondary stage input on V38 and a pair of stage outputs on V39 and V40.

1. Open Chrome and open the Kumo control page (it should be bookmarked).
2. Select the destination patch for your confidence monitor, V39. Now select which source you would like to send down V39 (if you want to match what is being projected, you would select "Program Roland", but if you want a different Roland input from what is being projected, you could use "Preview Roland" after routing that source through the Roland's bottom row. On the Roland, Preview will light up green while Program will light up red.)
3. Gather a Decimator and its power cable, SDI cable, HDMI cable, a monitor and its power cable, and any power strips or extension cords you need.
4. Place the monitor on stage with the Decimator near it and connect the HDMI output to the monitor's input using the HDMI cable.
5. Run the SDI cable from the Decimator's SDI Input to whatever AVP patch point is closest.
6. In the amp room, use the BNC patch to connect V39 to whichever patch point you chose. If an image doesn't appear on the monitor, double check the monitor video source and the Decimator configuration, or review the troubleshooting section above.

***
