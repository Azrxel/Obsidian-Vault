## Configure a Switch with Initial Settings
### The Boot System Command
- The Switch Attempts to automatically boot by using the information in the BOOT environment variable.
	 - If the this variable is not set the Switch attempts to load and execute the first executable file it can find
- The IOS Operating System then initializes the Interfaces using the Cisco IOS commands found in the startup-config file
	 - The startup-config file is called config.txt and is located in the flash
- In the example, the BOOT environment variable is set using the `boot system` global configuration mode command.
	- Notice the IOS is located in a distinct folder and the folder path is specified.
	- Use the command `show boot` to see the current IOS boot file is set to.
	
**`S1(config)# boot system flash:/c2960-lanbasek9-mz.150-2.SE/c2960-lanbasek9-mz.150-2.SE.bin`**

| Command                         | Definition                  |
| ------------------------------- | --------------------------- |
| boot system                     | The main command            |
| flash:                          | The storage device          |
| c2960-lanbasek9-mz.150-2.SE/    | The path to the file system |
| c2960-lanbasek9-mz.150-2.SE.bin | The IOS file name           |

### Switch LED Indicators
- System LED (<span style="color:rgb(77, 234, 255)">SYST</span>): Shows whether the system is receiving power and functioning properly.
- Redundant Power Supply LED (<span style="color:rgb(255, 192, 0)">RPS</span>): Shows the RPS status.
- Port Status LED (<span style="color:rgb(255, 255, 0)">STAT</span>): When <span style="color:rgb(0, 176, 80)">Green</span>, indicates port status mode is selected, which is the default.
  Port status can then be understood by the light associated with each port
- Port Duplex LED (<span style="color:rgb(198, 77, 255)">DUPLEX</span>): When <span style="color:rgb(0, 176, 80)">Green</span>, indicates port duplex mode is selected. 
  Port duplex can then be understood by the light associated with each port.
- Port Speed LED (<span style="color:rgb(102, 255, 71)">SPEED</span>): When <span style="color:rgb(0, 176, 80)">Green</span>, indicates port speed mode is selected.
  Port speed can then be understood by the light associated with each port
- Power over Ethernet LED (<span style="color:rgb(255, 82, 241)">PoE</span>): Present if the switch supports PoE.
  Indicates the PoE status on the switch
- The MODE button is used to move between the different modes - STAT, DUPLEX, SPEED, & PoE