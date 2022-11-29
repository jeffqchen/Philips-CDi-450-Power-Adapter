# Philips CD-i 450 Power Adapter

<img src="./Pics/01.jpg" width=800>
<img src="./Pics/02.jpg" width=400><img src="./Pics/03.jpg" width=400>

------
## Rambling

The Philips CD-i 450 has a weird PSU. It uses an RJ45 jack to connect to the console.

<img src="./Pics/cdi_psu.jpg" width=400>

Everybody familiar with ethernet cables knows the plastic tab on an RJ45 plug will snap off sooner or later. Then the plug will become loose and start falling out of the jack. While it might not be that devastating on a network connection, it is unacceptable for a power connection. Not to mention that over the decades, some consoles will be separated from its original PSU, and replacements are expensive while supplies being limited.

------
## Functionality

### Power Sources

<img src="./Pics/spec_01.jpg" width=400>

This adapter utilizes TWO **Center-Positive 5V** power adapters, with the plug dimension of **5.50mm OD (0.217") and 2.10mm ID (0.083")**.

**Do NOT** use a Y-adapter with a single power source or your adapter will short and die.

<img src="./Pics/spec_02.jpg" width=400><img src="./Pics/spec_03.jpg" width=400>

The one on the left requires 3.3A (16.5W). I call this the "beefy" one.

The one on the right is a weak one that any 5V adapter you can find will be more than capable to handle the job.

These power rating specs are the lowest requirements. You can go higher but not lower.

### Transmission Cable

<img src="./Pics/cable.jpg" width=400>

Use a **straight** RJ45 ethernet cable in short length. The wiring order on the two ends of the cable should be **exactly the same** or bad things will happen. It's easy to test with a meter if visual inspection is difficult.

### Usage

Plug everything in and use the power switch on the CD-i itself to turn the power on/off.

<img src="./Pics/final_led_off.jpg" width=400><img src="./Pics/final_led_on.jpg" width=400>

------
## Parts
- PCB - [Link](https://oshpark.com/shared_projects/HBbJdevy)
- [2x] PJ-002A Barrel Jack, OD 5.50mm / ID 2.10mm - [Link](https://github.com/jeffqchen/JeffParts/blob/main/Connectors/Barrel%20Jack/PJ-002A/info.md)
- 1705951 RJ45 Ethernet Jack, Female - [Link](https://github.com/jeffqchen/JeffParts/blob/main/Connectors/RJ45/Female/1705951/info.md)
- J104A2C5VDC.40S General Purpose Relay, DPDT, 5V/3A - [Link](https://github.com/jeffqchen/JeffParts/blob/main/Components/J104A2C5VDC.40S%20Relay/info.md)
- M3x20mm hex screw and nut - [Link](https://github.com/jeffqchen/JeffParts/blob/main/Parts/M2%20M3%20Hex%20Screw%20%26%20Nut/info.md)
- 3D Printed Case

**Optional Parts**
- 1N4148W Diode (for possible extending lifespan of relay coil)
- LEDs for power state indication
  - Two of each color, with their respective current limiting resistor (0805 size or smaller)
  - Typical LED forward voltage range from 2V to 3.2V. 100-150 Ohm resistors is a good choice.

### Power Sources

- "Beefy" WSU050-4000, 5V/20W, OD5.5mm/ID2.1mm, Triad Power Adapter - [Link](https://github.com/jeffqchen/JeffParts/blob/main/Power/WSU050-4000/info.md)
- WSU050-1500, 5V/7.5W OD5.5mm/ID2.1mm, Triad Power Adapter - [Link](https://github.com/jeffqchen/JeffParts/blob/main/Power/WSU050-1500/info.md) (but really, any 5V adapter will do)

------
## 3D Printing The Shell

Print the parts as shown in the following pics, with support.

<img src="./Pics/3dprint_shell.jpg" width=400>
<img src="./Pics/3dprint_lid.jpg" width=400>

------
## Assembly

### Populating Components

<img src="./Pics/solder.jpg" width=400>

Populate the PCB with parts. Trim the extra length of extruding legs but no need to go crazy.

#### LEDs
<img src="./Pics/leds.jpg" width=400>

D1 and D2 are for standby and D3 and D4 are for running. Choose your colors accordingly.

If in case one side does not light up, please check your power sources first as there might be a serious problem.

### Closing The Case

Fit into the bottom shell. Close the top shell over.

<img src="./Pics/assembly_01.jpg" width=400>

Drop the nut inside the cavity, then tighten the screwn from the bottom.

<img src="./Pics/assembly_02.jpg" width=400>

Drop in the top lid inside, fit one side in position first, then press and snap the other side into the slot.

This concludes the assembly.

<img src="./Pics/01.jpg" width=600>

<img src="./Pics/final_led_off.jpg" width=300><img src="./Pics/final_led_on.jpg" width=300>
