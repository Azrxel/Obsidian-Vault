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
- System LED (SYST): Shows whether the system is receiving power and functioning properly.
- Redundant Power Supply LED (RPS): Shows the RPS status.
- Port Status LED (STAT): When Green, indicates port status mode is selected, which is the default. 
snippets : 