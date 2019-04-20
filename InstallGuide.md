# WiiHDMI Install Guide
Follow this to install the WiiHDMI. It involes soldering to adjacent pins on a fine-pitch IC, so it's for people that are confident with their soldering skills.  
Before you start check if your Wii is compatible with WiiHDMI. This is easily done by opening the battery cover, the revision number is printed right there on the mainboard. [Supported revisions](https://github.com/wmi-0/wiihdmi#compatibility)  
The images have been resized to reduce the bandwidth required to load this page. High-res images of each step are located in pictures\installguide if necessary.

# Step 1: Disassembly
Follow this guide to disassemble your Wii: https://www.ifixit.com/Guide/Nintendo+Wii+Motherboard+Replacement/3460  
This is more complex than a typical console teardown, take your time and pay attention to the different screw sizes. I suggest grouping them by the corresponding step number of the iFixit guide.

# Step 2: WiiHDMI install
Make sure that both PCBs are aligned straight and are placed as close as possible to the Wii mainboard. Use solder wick to remove some of the solder on the GND pins if necessary.  
![step_2_1_small.jpg](/pictures/installguide/step_2_1_small.jpg?raw=true)

Solder the Main PCB and HDMI PCB to the board.  
![step_2_2_small.jpg](/pictures/installguide/step_2_2_small.jpg?raw=true)

Connect the pads to the AVE-RVL.  
![step_2_3.jpg](/pictures/installguide/step_2_3.jpg?raw=true)

When finished it should look something like this.  
![step_2_4_small.jpg](/pictures/installguide/step_2_4_small.jpg?raw=true)

Now we just need to connect the solder pad for the gamepad to TP27, which is Gamecube controller port 1.  
![step_2_5_small.jpg](/pictures/installguide/step_2_5_small.jpg?raw=true)

And finally insert the ribbon cable and fold appropriately. Don't risk breaking the FFC by folding it too tight, there's plenty of space between the mainboard and shielding.  
![step_2_6_small.jpg](/pictures/installguide/step_2_6_small.jpg?raw=true)

Now it's a good idea to test if the installation was successful. Place the top RF shield back on, connect the drive and place a piece of plastic or paper under the drive to avoid shorting something.
Connect power and the Mini-HDMI cable. If everything went well you should be greeted by the Wii menu.

# Step 3: Modifications
The bottom RF shield needs to be modified to allow for some space for the added boards. Use some pliers to wiggle or cut off the marked sections.  
![step_3_1_small.jpg](/pictures/installguide/step_3_1_small.jpg?raw=true)

Like so.  
![step_3_2_small.jpg](/pictures/installguide/step_3_2_small.jpg?raw=true)

Now we need to modify the bottom plastic shell to fit the Mini-HDMI connector. Mark the edges of the connector with a pen.  
![step_3_3_small.jpg](/pictures/installguide/step_3_3_small.jpg?raw=true)

And use a file to create a cutout to fit the connector.  
![step_3_4_small.jpg](/pictures/installguide/step_3_4_small.jpg?raw=true)

On the other side mark the position of the Switch and the IR sensor. Then drill a small hole for each at the approximate position.  
![step_3_5_small.jpg](/pictures/installguide/step_3_5_small.jpg?raw=true)

Also cut of a part of the sponge the power pins press against for it to clear the WiiHDMI PCB.  
![step_3_6_small.jpg](/pictures/installguide/step_3_6_small.jpg?raw=true)

The upper part of the case needs to be modified as well. Put it on top, mark the position of the connector and file away.  
Depending on the placement of the HDMI PCB it's possible that the inner wall of the case needs to be made a bit thinner for it to clear the PCB and allow the case to close properly.  
![step_3_7_small.jpg](/pictures/installguide/step_3_7_small.jpg?raw=true)

After all the work it should look something like this.  
![step_3_8_small.jpg](/pictures/installguide/step_3_8_small.jpg?raw=true)

# Step 4: Reassembly
Follow the iFixit guide in reverse order. If you've kept track of the screws it should be pretty easy this time.
