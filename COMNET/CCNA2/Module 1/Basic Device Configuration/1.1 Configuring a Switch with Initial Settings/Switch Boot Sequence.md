After a Cisco Switch is powered on, it goes through the following 5-Step Boot Sequence:
### Step 1:
First, the Switch loads a Power-On Self-Test (POST) program stored in the ROM.
POST checks the CPU subsystem. It tests the CPU, DRAM, and the portion of the flash device that makes up the flash file system.

### Step 2: 
Next, the Switch loads the boot loader software.
The Bootloader is a small program stored in ROM that is run immediately after POST successfully completes.

### Step 3: 
The Bootloader performs low-level CPU initialization.
It Initializes the CPU registers, which control where Physical Memory is mapped, the quantity of Memory, and its Speed.

### Step 4:
The Bootloader initializes the flash file system on the System Board.