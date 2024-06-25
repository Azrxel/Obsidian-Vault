Windows 10 Boot Sequence after the Boot Manager (bootmgr.exe) loads
	Steps:
	1. The Windows bootloader <span style="color:rgb(0, 176, 240)">Winload.exe</span> <u>loads</u>
	2. <span style="color:rgb(0, 176, 240)">Ntoskrnl.exe</span> and <span style="color:rgb(0, 176, 240)">hal.dll</span> are <u>loaded</u>
	3. <span style="color:rgb(0, 176, 240)">Windload.exe</span> reads the Registry, chooses a hardware profile, and loads the device drivers
	4. <span style="color:rgb(0, 176, 240)">Ntoskrnl</span> takes over the process

API Functions within the Windows 10 Environment
	1. <span style="color:rgb(255, 255, 0)">OpenGL</span>:
	   This is a cross-platform standard specification for multimedia graphics
	2. <span style="color:rgb(255, 255, 0)">DirectX</span>
	   Collection of APIs related to the multimedia tasks for Microsoft Windows
	3. <span style="color:rgb(255, 255, 0)">Windows APIs</span>
	   Allows applications from older versions of Windows to operate on newer versions  
	4. <span style="color:rgb(255, 255, 0)">Java APIs</span>
	   Collection of APIs related to the Development of Java programming

2 Tools to used to transfer Data & Settings from an Old Windows Computer to a New Computer
	1. <span style="color:rgb(255, 192, 0)">Windows Easy Transfer</span>
	2. <span style="color:rgb(255, 192, 0)">User State Migration Tool</span> 
	#Explanation: 
		When a new operating system is being installed, existing user data and settings need to be migrated from the old to the new operating system. The User State Migration Tool and the Windows Easy Transfer Tool are available to perform this task on the Windows Vista, 7, and 8 operating systems

#Scenario A user wants to extend a primary partition formatted with the NTFS file system with the unallocated space on the hard disk. What must the user do after the primary partition is extended to make it usable?
	1.<span style="color:rgb(198, 162, 226)">Convert the Disk Type to Dynamic</span>
	#Explanation: 
		A partition must be formatted with the NTFS file system in order to extend it by using the unallocated space on the disk. Once the partition has been extended, the disk type must be converted to a dynamic disk in order for the new partition to be accessible

Why a full format more beneficial than a quick format when preparing for a clean OS Installation
	1. <span style="color:rgb(198, 162, 226)">A full format will delete files from the disk while analyzing the disk for drive errors</span>
	   #Explanation: 
		   A full format removes files from a partition while scanning the disk for bad sectors. A quick format will remove files from a partition but does not scan a disk for bad sectors.

#Scenario: A Technician wishes to prepare the computers in the network for a disaster recovery. The network Consists of variety of Desktops and laptops from different vendors.  All the computers are running either a 32 or 64 - Bit version of Windows 10 Pro. How would the technician prepare the recovery media?
	1. Prepare individual recovery discs for all the computers
	#Explanation: 
		All the PCs are from different vendors and thus have dissimilar hardware configurations. Furthermore, all the PCs have a variety of 32-bit Windows 10 and 64-bit Windows 10. Because the PCs have different versions of the OS and dissimilar hardware, you cannot use the same image on all the PCs . In order to use a single image, Sysprep must be used to strip out machine specific information like the SID, and all PCs must have the same hardware configuration and the same version of the Windows operating system.

### RAID Levels

|                              Level                               |                                                       Description                                                       |               Minimum # of Drives               |
| :--------------------------------------------------------------: | :---------------------------------------------------------------------------------------------------------------------: | :---------------------------------------------: |
|        <span style="color:rgb(255, 192, 0)">RAID 0</span>        |                                  <span style="color:rgb(255, 192, 0)">Striping</span>                                   |  <span style="color:rgb(255, 192, 0)">2</span>  |
|        <span style="color:rgb(0, 176, 240)">RAID 1</span>        |                                  <span style="color:rgb(0, 176, 240)">Mirroring</span>                                  |  <span style="color:rgb(0, 176, 240)">2</span>  |
|                            ~~RAID 2~~                            |                                   ~~Striping with Hamming Code for Error Correction~~                                   |                                                 |
|                            ~~RAID 3~~                            |                     ~~Striping with <span style="color:rgb(0, 176, 240)">Dedicated</span> Parity~~                      |                                                 |
|                            ~~RAID 4~~                            |                     ~~Striping with <span style="color:rgb(0, 176, 240)">Dedicated</span> Parity~~                      |                                                 |
|        <span style="color:rgb(255, 255, 0)">RAID 5</span>        |      <span style="color:rgb(255, 255, 0)">Striping</span> with <span style="color:rgb(255, 255, 0)">Parity</span>       |  <span style="color:rgb(255, 255, 0)">3</span>  |
|       <span style="color:rgb(198, 162, 226)">RAID 6</span>       | <span style="color:rgb(198, 162, 226)">Striping</span> with <span style="color:rgb(198, 162, 226)">Double Parity</span> | <span style="color:rgb(198, 162, 226)">3</span> |
| <span style="color:rgb(146, 208, 80)">RAID 10</span> <br>(0 + 1) |     <span style="color:rgb(146, 208, 80)">Mirroring</span> & <span style="color:rgb(146, 208, 80)">Striping</span>      | <span style="color:rgb(146, 208, 80)">4</span>  |

### 6 Steps of Troubleshooting

| Steps  | Step taken                                                                       |
| ------ | -------------------------------------------------------------------------------- |
| Step 1 | Identify the Problem                                                             |
| Step 2 | Establish a theory of Probable Cause                                             |
| Step 3 | Test the Theory to Determine the Cause                                           |
| Step 4 | Establish a Plan of Action to Resolve the Problem and Implement the Solution     |
| Step 5 | Verify Full System Functionality and if Applicable Implement Preventive Measures |
| Step 6 | Document Findings, Action, and Outcomes                                          |

### Cloud Computing Services

|           Service            | Description                                                                                                                                                                                                                                                             |
| :--------------------------: | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| PAAS (Platform As A Service) | Provides a <span style="color:rgb(0, 176, 240)">collaborative environment</span> where multiple developers can <span style="color:rgb(0, 176, 240)">create software</span> and <span style="color:rgb(0, 176, 240)">host an application</span> through a Cloud Provider |
|             IAAS             |                                                                                                                                                                                                                                                                         |
|             SAAS             |                                                                                                                                                                                                                                                                         |

### SDRAM Memory Types

| Type                                                     | Features                                                                                                                            |
| :------------------------------------------------------- | :---------------------------------------------------------------------------------------------------------------------------------- |
| <span style="color:rgb(146, 208, 80)">DDR</span> SDRAM   | <span style="color:rgb(146, 208, 80)">148</span> Connector Pins, Supports Two Writes, and Two Reads per CPU Clock Cycle             |
| <span style="color:rgb(255, 255, 0)">DDR2</span> SDRAM   | <span style="color:rgb(255, 255, 0)">240</span> Connector Pins, Consumes <span style="color:rgb(255, 192, 0)">1.8V</span> of Power  |
| <span style="color:rgb(255, 255, 0)">DDR3</span> SDRAM   | <span style="color:rgb(255, 255, 0)">240</span>  Connector Pins, Consumes <span style="color:rgb(0, 176, 240)">1.5V</span> of Power |
| <span style="color:rgb(198, 162, 226)">DDR4</span> SDRAM | <span style="color:rgb(198, 162, 226)">288</span> Connector Pins, has Advanced Error Correction Features Available                  |

### Problems and Solutions for Computers

| Problem                                                                                                | Solution                                                                                                             |
| ------------------------------------------------------------------------------------------------------ | -------------------------------------------------------------------------------------------------------------------- |
| The Motherboard capacitors are distended, swollen, emitting residue, or bulging                        | Replace The Motherboard                                                                                              |
| The User can hear the fans spinning but the PC will not start and there are no beeps from the speaker  | Check for faulty cables, damaged or mis-seated CPU, or other MOBO components prior to replacing the MOBO if required |
| After upgrading the single core CPU to a Dual Core CPU, only one CPU Graph is seen in the Task Manager | Update The Bios Firmware                                                                                             |
| The Computer does not display any Video after installing a new PCIe Video Card                         | Connect the Auxiliary Power Cable for the Adapter Card                                                               |

### Port Numbers & Services

|                      Port #                      | Services                                              |
| :----------------------------------------------: | ----------------------------------------------------- |
|  <span style="color:rgb(255, 192, 0)">22</span>  | <span style="color:rgb(0, 176, 240)">SSH</span>       |
|  <span style="color:rgb(255, 192, 0)">23</span>  | <span style="color:rgb(0, 176, 240)">Telnet</span>    |
|  <span style="color:rgb(255, 192, 0)">25</span>  | <span style="color:rgb(0, 176, 240)">SMTP</span>      |
|  <span style="color:rgb(255, 192, 0)">53</span>  | <span style="color:rgb(0, 176, 240)">DNS</span>       |
| <span style="color:rgb(146, 208, 80)">137</span> | <span style="color:rgb(198, 162, 226)">NetBIOS</span> |
| <span style="color:rgb(146, 208, 80)">143</span> | <span style="color:rgb(198, 162, 226)">IMAP</span>    |
| <span style="color:rgb(146, 208, 80)">161</span> | <span style="color:rgb(198, 162, 226)">SNMP</span>    |
| <span style="color:rgb(146, 208, 80)">389</span> | <span style="color:rgb(198, 162, 226)">LDAP</span>    |
| <span style="color:rgb(146, 208, 80)">427</span> | <span style="color:rgb(198, 162, 226)">SLP</span>     |

### ACPI Power States

| State | Description                                                                        |
| :---: | ---------------------------------------------------------------------------------- |
|  S0   | PC on, CPU Running                                                                 |
|  S1   | CPU & RAM Rx Power, but unused devices powered on                                  |
|  S2   | CPU off, but RAM is Refreshed                                                      |
|  S3   | CPU is off, and RAM set to slow Refresh Rate (Suspended Mode)                      |
|  S4   | CPU & RAM off, Contents of RAM have been saved to temporary file on the Hard Drive |
|  S5   | Computer is Off                                                                    |

### Windows Boot Sequence
1. Power on Self Test (POST)
2. POST for each adapter card that has a BIOS  
3. BIOS reads the MBR
4. MBR takes over control of the boot process and starts BOOTMGR  
5. BOOTMGR reads the Boot Configuration Data file to know which OS to load and where to find the OS on the boot partition 
	5.1. **<span style="color:rgb(255, 255, 0)">BOOTMGR</span> invokes <span style="color:rgb(255, 255, 0)">W<span style="color:rgb(255, 255, 0)">INL</span>OAD.EXE</span> in order to load the <span style="color:rgb(255, 255, 0)">N</span><span style="color:rgb(255, 255, 0)">TOSKRNL.EXE</span> file and <span style="color:rgb(255, 255, 0)">HAL.DLL</span>**
	5.2. **<span style="color:rgb(255, 255, 0)">BOOTMGR</span> reads the registry files and loads device drivers** 
	5.3. **<span style="color:rgb(255, 255, 0)">NTOSKRNL.EXE</span> starts the <span style="color:rgb(255, 255, 0)">WINLOGON.EXE</span> program and displays the Windows login screen**  
At this point, the NT kernel takes over. The NT kernel is the heart of all Windows operating systems. The name of this file is NTOSKRNL.EXE. It starts the login file called WINLOGON.EXE and displays the Windows Welcome screen.