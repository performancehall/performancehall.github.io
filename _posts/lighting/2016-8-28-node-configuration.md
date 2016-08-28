---
layout: post
title: Node Configuration Instructions
permalink: /lighting/node-configuration.html
---

1. Plug the node into the lighting network and write down the ip address taped to the side of the node

2. Find a Mac (If you're using a PC, you're on your own...)

3. Open System Preferences

4. Go to the Network Preferences page

5. Move the “Auditorium” Wi-Fi network

6. Click on Advanced towards the bottom right corner of the window

7. Go to the TCP/IP page

8. In the drop down menu where it says “Configure IPv4” select “Manually”

9. Give the computer an ip address of `192.168.0.199` (or any other ip address within the
lighting network but not used by an entity on that network)

10. Give the computer a Subnet Mask of `255.255.255.0`

11. Click Ok and then click Apply

12. Open Firefox (other browsers are less successful at interacting with the strand
interface)

13. Type in the ip address of the mode where you would enter a web address + /mini/

    * If the ip address is: `192.168.0.72`
    * Type in: `192.168.0.72/mini/`

14. There are only a few things that you should be changing in this screen, depending
upon what you are configuring the node to do:

    * You can change whether the ports (DMX A and DMX B) output or input DMX by
going to their respective pages within this screen by clicking on them and then
selecting DMX in from the drop-down menu

    * You can change what DMX universe (set of 512 DMX channels—usually we’ll just
be using universes one and two to give the hall a total of 1024 addressable channels of lighting control) each port corresponds to by changing the “Netslot” field value of each port along the bottom of the window.

        * To put a DMX port (A or B) in Universe 1, enter “1” for the “Netslot” For Universe 2, you would enter 513 for the “Netslot”

    * If you reconfigure the node, make sure to change the label for each DMX port to reflect what it is doing, (i.e. if you configure a port to be DMX in second universe, change the label to DMX IN U2)

15. Click Update to update the node with the changes you made. The password is `2606`. Go back to the DMX A and DMX B pages to make sure the desired changes held.

16. After reconfiguring the node, for the changes to take effect, you frequently have to reboot the node by unplugging it from ethernet and then plugging it back in!

17. You’re done! To make your computer connect to the regular internet again, go back to the Configure IPv4 drop down menu in system preferences and change it back to “Using DHCP” and apply the changes.
