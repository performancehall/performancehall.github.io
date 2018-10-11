---
layout: post
title: Archival Recording Standards
permalink: /recording/archival-recording-standards.html
---

## Archival Audio Recording Instructions and Monitor/Page/Hearing Assist

**Archival Recording in the Hall**  
Setting up the Audio Console (Venue SC48):

1. Depending on the preset you use, the ceiling microphone pair that we use for recording shows may be soft-patched differently, but they should always be patched into inputs 30 and 31. There are many ways to set up this patch in order to record shows, however I will detail two main ways, the first being the conceptually simple but lower quality method using direct outputs, and the second being the slightly more complicated but higher quality method using matrices.
2. Using direct outs
	*  The easiest and quickest way to get recording setup is to patch the direct outputs of the hanging house mic left and right inputs to the firewire output that goes into the Mac Mini. To do this, select the “PATCHBAY” tab on the SC48 monitor, within this tab, there should be four sub-tabs labeled “INPUTS,” “OUTPUTS,” “DIRECTS” and “INSERTS.” Select the “DIRECTS” sub-tab, and within this sub-tab, select the “PROTOOLS” subtab which can be found among the two other types of Hardware tabs (FOH and STAGE). For all practical purposes, PROTOOLS here refers to the Firewire cable that connects the Mac Mini to the Venue. Alongside the left edge of the patchbay grid you should see another set of tabs representing the types of channels available for patching based on your selection of the previous tabs. Make sure “CHANNELS” is selected, as opposed to “FX RETURNS.” We use Firewire outputs 1 and 2 as our recording outputs that go into the Mac Mini. Scroll down the patchbay grid until you find your hanging house mic left and right channels, and then patch each one to Firewire 1 and 2 accordingly. Lastly DO NOT FORGET to go back to the INPUTS tab at the top of the SC48 monitor, select each hanging house mic input channel, and turn on and turn up the direct output on each channel. If you forget to do this you will not get anything out of your direct outputs. (Turn the direct out on by clicking the IN graphic and turn it up by turning up the graphic encoder just above this virtual button)
	* DO NOT FORGET to gain your hanging house mics appropriately. I find that a gain of about 10 o’clock seems to work well for any type of show. Optimally, you would gain the mics enough to get the incoming signal as close to 0 dB as possible without going over, or clipping. It never hurts to be too quiet, while on the other hand, clipping distortion is irreversible, so it is always better to err on the side of caution and leave your hanging house mics gained less if you think things may get loud later in the show. If you can remember, make an effort to look at the incoming signal to these channels during your show to make sure you are not clipping. Adjust your gains on these channels appropriately.
3. Using Matrices
	* This method uses matrices to send not only the hanging house mic feed into the mac but also takes a split of everything being sent out of your main outs and sends that as well. Thus it is a higher quality option for recording as opposed to simply taking the ambient house mic feed through direct outputs. Since we are sending a stereo output to the Mac, we need to set up a stereo matrix pair. Matrices 1-6 are always in use by the board, as they feed the Line arrays, subs booster, and surrounds, so you will use matrices 7 and 8. To stereo pair these matrices, go to the OPTIONS tab, and then to the BUSSES subtab. Within this tab you can stereo pair auxes and matrices. Go into configuration mode (either by hitting the red button labeled “Config” in the upper left center of the board or by double clicking the SHOW label at the bottom of the SC48 monitor), and then hit the EDIT button in the matrix section of the BUSSES subtab. Hit the checkmark above 7 and 8 to stereo pair them. Next, you need to set up these matrices so that they take the correct configuration of inputs and outputs that we want sent to the recording. Go to the OUTPUTS tab and select either one of your matrices. Inside the matrix mixer you will find 12 possible input channels to the matrix, on the right you will see your left-center-right options. We want to send the hanging house mics to the mac through this matrix, as well as the left-center-right outputs of the board. Turn the Left-Right and Center channels in the matrix mixer on and up via the controls beneath the virtual meter on each channel. Left-Right should be stereo paired, denoted by the checkbox beneath even-odd pairs of channels. If not then simply hit the corresponding checkbox. When any two input channels are stereo paired in the matrix mixer turning one on and up will automatically do so for its stereo partner. Once you turn Left-Right and Center on and up, hit the red user assign button in the matrix mixer. This will bring up the user assign tab. Preferably find two unused user assign channels, and from the drop down set them to your hanging house mic left and right input channels respectively. If all the user assign channels are in use, then change two that you don’t need for the current show (note that changing these user assigns will change them for any other matrices using those user assigns, so be sure you don’t need them before you change them). Hit the user assign button again to exit the user assign tab. Go to the first two channels in the matrix mixer, and from the dropdown box just above the virtual meter for each channel navigate to your hanging house mic left and right user assigned channels. Since these two channels constitute a stereo pair, hit the checkbox beneath these channels to link them. This should bring up a panning option, make sure it is set correctly (pan HHL all the way left and HHR all the way right), and then turn on and up the two channels. If you did this correctly your meters for these hanging house mic channels in the matrix mixer should be showing signal if there is any noise in the hall. Theoretically, since you stereo paired the two matrices, everything you just did for this matrix should have been automatically copied over to matrix 8, or vice versa if you started with 8, but just to be sure you should always check to see that everything is correct in both matrices. They should simply be identical copies of each other. Turn up these matrix faders on your board to unity (0 db) and then navigate to the PATCHBAY tab on-screen. We now need to patch these matrices. We want to send them to Firewire outputs 1 and 2 respectively. In the PATCHBAY tab, click the OUTPUTS subtab, and the PROTOOLS subtab within that. Select MATRIXES from the selection of output type tabs on the left edge of the virtual patchbay display. Find Matrix 7 and 8 and patch them to Firewire 1 and 2 respectively. Make sure your matrix 7 and 8 channels are unmuted and turned up.
	* NOTE that if you are using this method for recording, it is highly recommended that you MONITOR your recording outputs in order to not only gain your hanging house mics properly (see Using direct outs part (b) above) but also to get a good mix between these ambient signals and the onstage microphone signals being sent to your mains. In general, the ambient recordings should be quieter, placed in the background behind the main outputs. To monitor the mix, take the headphones that should be hanging underneath the desk where you are sitting and plug them into the headphones input on the board (beneath the front lip of the board towards the right side). Hit the AFL button on one of the matrices you are using for the recording, and use the headphones volume encoder on the upper right hand corner of the board to send the recording feed to your headphones and control the volume in your cans respectively. Adjust the mix as necessary. Again, it is always better to err on the side of caution and keep your hanging house mic feed on the quiet side if you are unsure about the mix or whether or not it will hold during the actual show. If you get downtime during the show you can always monitor the mix and adjust accordingly.

Setting up the Mac Mini:

1. Turn on the Mac Mini and its monitor display
2. Click on your empty desktop
3. Choose “Go” in from the options tab at the top of the display
4. Select “Applications”
5. Open “Microwave”

Setting up your session:

1. Change the Sample Rate to 44100
2. Change the bit depth to 24 bit
3. Change the channels to stereo if showing mono
4. Click “Create”
5. Name your session according to the naming protocol: Year.Month.Date_Show_Engineer
6. Click the arrow next to the file name to drop down the filing menu
7. Save the file under “Documents” -> “PH_Recordings”

Testing the recording during rehearsal:

1. Press the record button to enable recording (large red circle) while making noise
2. Press the same record button to stop recording
3. If you see a very slight waveform, it means your recording is working, but you want more signal
4. Gain the hanging house mics until you see a better waveform. Congrats! You’ve got a recording going.
5. Drag the timing bar back to the beginning of your recording; it will allow you to record over your test
Record the show: Press Record both before and after the show

Normalize, Gain, Normalize:

1. From the drop down menu at the top of the screen choose “Effects” then “Normalize”; allow it to process
2. Next, also under “Effects”, choose “Multiband Compressor” and press “Apply” on the pop up window
3. Normalize again by repeating step 1: “Effects” and “Normalize”
4. Choose “File” -> “Export”
5. Ensure that the Output File Format is MPEG 2 Audio Layer III (.mp3) and press “OK”
6. Name the file the same way you named the session: Year.Month.Date_Show_Engineer
7. Click the arrow next to the file name to drop down the filing menu
8. Save the file under “Documents” -> “PH_Recordings”

Send the file to erinbrenner@uchicago.edu:

1. Open Chrome (using the same method you used to open Microwave or from the dock below)
2. Go to the website WeTransfer.com
3. Upload the recording -> enter Erin’s email address -> enter your email address -> press Send


Naming Convention: Year.Month.Date_Show_Engineer.mp3  
*Example*:    14.8.31_ThirdCoastPercussion_Remy.mp3  
*Example*:    15.2.24_MEME_Jace.mp3

**Troubleshooting the Monitor/Page/Hearing Assist Feed**

Hard Patch

* The monitor/page/hearing assist feed is fed directly from the center hanging house mic in the performance hall. The microphone is plugged into M29 in the center AVP 202 on catwalk 1. In the patchbay this is patched into the hear assist input.

Presonus

* The signal from the microphone is sent through the Presonus Studio One Channel Preamp in the top center rack of the amp room. This unit also feeds the hanging house mic +48 volts phantom power, without which it will not work properly. The other settings and parameters on this preamp channel strip are set according to what makes the /monitor page feed sound best, so please do not touch any of these other controls. The only thing you should ever have to touch on this unit is the 48 volts button, which occasionally gets turned off by accident.

Crestron Control Unit and DSP

* The signal from the preamp is sent to a Crestron control unit and some DSPs. The Crestron Control Unit can be found towards the bottom of the center rack in the amp room and is labeled CU-11. The last step in the troubleshooting process after checking the hard patch and the Presonus unit is to take a look at this control unit and verify that it is working properly. If the MSG and or LNK lights are not on, or it looks like the London DSPs immediately below this unit do not seem to be receiving signal, then you may need to try doing a software or hardware reset in the Crestron Control Unit. If you think you need to do this, notify a supervisor first and get his or her approval to do so. Always try doing a software reset first. This can be done by pressing the inset button on the control unit labeled SW-R. If this does not fix the problem, trying hit the other inset button just to the left of this one labeled HW-R. This will force the unit into a hardware reset.
