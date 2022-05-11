# UM-80 Assembly Guide

## **Content of UM-80 Kit**

<a href="images/Content.jpg">
<img src="images/Content.jpg" width="400">
</a>

**Printed Parts** 
- 2 x Top Cases
- 2 x Rear Covers
- 2 x Side Panels
- 1 x Rotary Encoder Knob

**Electronics**
- 1 x Main PCB (Left & Right)
- 1 x OLED Screen PCB
- 1 x OLED Screen
- 2 x 4 Pins Sockets
- 1 x 4 Pins Cable
- 1 x Encoder
- 120 x SK6812MINI RGB LED (Only 100 are required)
- 90 x Hot swap sockets (Only 87/88 are required)
- 2 x TRRS PJ-320A

**Fasteners**
- 30 x M2 3mm screws (Only 26 are required)
- 15 x M2 3mm Standoffs (Only 13 are required)
- 15 x M2 washers (Only 13 are required)
- 20 x M3 5mm screws (Only 16 are required)
- 5 x M3 16mm screws (Only 4 are required)
- 5 x M3 25mm screws (Only 4 are required)

**Miscellaneous**
- 1 x FR4 Plates (Left & Right)
- 8 x Rubber feet



---


## **Test the PCBs before soldering**

<a href="images/PCB_Test.jpg">
<img src="images/PCB_Test.jpg" width="400">
</a>

All PCBs are tested prior shipping, but it is good practice to make sure they are working before soldering. Both PCBs should be recognised as keyboard input device when connected to a computer. Plug in one half and test by shorting switch pins with tweezers. After testing one half, disconnect the first and test the other half.

**Don’t panic if the right side PCB outputs the wrong key for that switch location or not registers some of the keys, as the firmware is set to left as master. As long as both halves produce some output you have verified the PCBs are working.**



## **Assembling the Main PCBs**

<a href="images/Panel_led.jpg">
<img src="images/Panel_led.jpg" width="400">
</a>

**_Blue = In-switch LEDs_**

**_Orange = Panel LEDs_**

There are 41 in-switch and 7 panel LEDs on the left half. 45 in-switch (46 for split backspace) and 7 panel LEDs on the right side.


## **Panel LEDs**

<a href="images/PanelLEDLens.jpg">
<img src="images/PanelLEDLens.jpg" width="400">
</a>
<a href="images/PenalLEDMarking.jpg">
<img src="images/PenalLEDMarking.jpg" width="400">
</a>

To solder side panel LEDs, the LED lens should be facing up. Align the marking on the PCB and the LED then solder. Repeat the same process for the remaining side panel LEDs.

## **In-switch LEDs**

<a href="images/SwitchLEDMarking_A.jpg">
<img src="images/SwitchLEDMarking_A.jpg" width="400">
</a>
<a href="images/SwitchLED_B.jpg">
<img src="images/SwitchLED_B.jpg" width="400">
</a>

To solder in-switch LEDs, the LED lens should be facing down. Align the markings on the PCB and the LED then solder. Repeat the same process for the remaining in-switch LEDs.


<a href="images/Layout_Left.jpg">
<img src="images/Layout_Left.jpg" width="400">
</a>
<a href="images/Layout_Right.jpg">
<img src="images/Layout_Right.jpg" width="400">
</a>

When soldering LEDs for Spacekey on the left and Backspace on the right, pick one of the two layouts shown above. Be sure to only solder one layout.

## **Hot swap sockets**
<a href="images/08_Hotswap_A.jpg">
<img src="images/08_Hotswap_A.jpg" width="400">
</a>

Place sockets as shown in the photo. When soldering sockets for Spacekey on the left and Backspace on the right, refer to your chosen layout from the previous step for correct placement. Be sure to only solder sockets to one layout.

<a href="images/RightHowswap_A.jpg">
<img src="images/RightHowswap_A.jpg" width="400">
</a>

There are 4 sockets on the edge of the right half that need modification prior to soldering.

<a href="images/RightHowswap_B.jpg">
<img src="images/RightHowswap_B.jpg" width="400">
</a>
<a href="images/RightHowswap_C.jpg">
<img src="images/RightHowswap_C.jpg" width="400">
</a>

Spread the right pins of the socket as shown in the photo and then solder.


## **TRRS Jacks**
<a href="images/TRRS_A.jpg">
<img src="images/TRRS_A.jpg" width="400">
</a>
<a href="images/TRRS_B.jpg">
<img src="images/TRRS_B.jpg" width="400">
</a>

Place the jack on the underside of the PCB (the same side you just soldered sockets to) then solder.

## **OLED Screen Connector**
<a href="images/OLEDSocket_A.jpg">
<img src="images/OLEDSocket_A.jpg" width="400">
</a>

OLED screen connector is located on the left half.

<a href="images/OLEDSocket_B.jpg">
<img src="images/OLEDSocket_B.jpg" width="400">
</a>
<a href="images/OLEDSocket_C.jpg">
<img src="images/OLEDSocket_C.jpg" width="400">
</a>

Insert it on the underside of the PCB and then solder.

## **Buzzer**
_Optional, AST1109MLTRQ buzzer is not included in the kit_

<a href="images/Buzzer_A_L.jpg">
<img src="images/Buzzer_A_L.jpg" width="400">
</a>
<a href="images/Buzzer_A_R.jpg">
<img src="images/Buzzer_A_R.jpg" width="400">
</a>

Buzzers are located on the top sides of each PCB. Only solder a buzzer on the master half (Left half by default. Only solder the buzzer to the half that will be plugged into your PC via USB-C).

- _Audio is not enabled by default._

- _QMK does not support speaker on the on slave half._

- _Audio features take a large amount of memory, some other features may have to be disabled to allow space for it._

- _Buzzer is wired to IO pin B6._

<a href="images/Buzzer_B.jpg">
<img src="images/Buzzer_B.jpg" width="400">
</a>
<a href="images/Buzzer_C.jpg">
<img src="images/Buzzer_C.jpg" width="400">
</a>

AST1109MLRQ is non-polarity, solder anyway up.


---
## **Test the PCBs**


Connect both halves with TRRS cable **_first_**, and then connect USB cable to the **_left_** **_half_**.

**DO NOT PLUG/UNPLUG TRRS CABLE WHEN POWER IS ON (I.E. WHEN USB CABLE IS CONNECTED), IT CAN SHORT THE CONTROLLER.**

Check that all LEDs are working before proceeding to the next step.

### **Troubleshooting LEDs**

<a href="images/LEDOrder_L.jpg">
<img src="images/LEDOrder_L.jpg" width="400">
</a>
<a href="images/LEDOrder_R.jpg">
<img src="images/LEDOrder_R.jpg" width="400">
</a>

The LEDs are wired in series, see photos for the order.

If some of the LEDs do not light up or appear to be faulty, it’s most likely that something is wrong with the adjacent LEDs in the series.
For example, if LED 24-39 doesn’t light up, check LED 23 and 24.
- Check solder joints

- Make sure there is a capacitor, it may have got knocked off during handling

- It’s not unusual to encounter a faulty RGB LED, replace it.

- Make sure the right side is connected via TRRS cable.

Once all LEDs are working, move on to the next step

---

## **Encoder**
<a href="images/Encoder_A.jpg">
<img src="images/Encoder_A.jpg" width="400">
</a>

Encoder is located on the right half.

<a href="images/Encoder_B.jpg">
<img src="images/Encoder_B.jpg" width="400">
</a>
<a href="images/Encoder_C.jpg">
<img src="images/Encoder_C.jpg" width="400">
</a>

Insert encoder to the front of the PCB, solder it from the underside of the PCB.

## **Stabilisers**

<a href="images/Stab_A.jpg">
<img src="images/Stab_A.jpg" width="400">
</a>
<br>
<a href="images/Stab_B.jpg">
<img src="images/Stab_B.jpg" width="400">
</a>
<a href="images/Stab_C.jpg">
<img src="images/Stab_C.jpg" width="400">
</a>

When installing screw-in stabiliser for Spacekey on the left half, use a washer/electrical tape to isolate the screw and the LED contacts to prevent shorting.

## **Mounting PCB to plate**

<a href="images/PlateMountL.jpg">
<img src="images/PlateMountL.jpg" width="400">
</a>
<a href="images/PlateMountR.jpg">
<img src="images/PlateMountR.jpg" width="400">
</a>

There are 6 mounting points on the left side and 7 points on the right side.

<a href="images/StandOff_A.jpg">
<img src="images/StandOff_A.jpg" width="400">
</a>
<a href="images/StandOff_B.jpg">
<img src="images/StandOff_B.jpg" width="400">
</a>

Secure the standoffs to the plate with washers and M2 screws.

<a href="images/Switch_B.jpg">
<img src="images/Switch_B.jpg" width="400">
</a>

Insert switches to plate and PCB. Switches should seat flush on the PCB. 

<a href="images/PCBMountholes_L.jpg">
<img src="images/PCBMountholes_L.jpg" width="400">
</a>
<a href="images/PCBMountholes_R.jpg">
<img src="images/PCBMountholes_R.jpg" width="400">
</a>

Secure PCB to plate with M2 screws. 


---
## **Test the PCBs**


Connect both halves with TRRS cable **_first_**, and then connect USB cable to the **_left_** **_half_**.

**DO NOT PLUG/UNPLUG TRRS CABLE WHEN POWER IS ON (I.E. WHEN USB CABLE IS CONNECTED), IT WILL SHORT THE CONTROLLER.**

Confirm that all switches and the encoder are working before proceeding to the next step.

### **Troubleshooting Encoder/Switches**

**Encoder**
- Check solder joints.
- Make sure there is a diode, it may have got knocked off during handling.

**Switches**
- Dismount the switch and check for bent pins, straighten the pins with pliers if necessary.
- Check hot swap socket solder joints.
- Check for diode on near the switch, it may have got knocked off during handling.

---

## **Soldering OLED screen PCB**

<a href="images/OLED_PCB.jpg">
<img src="images/OLED_PCB.jpg" width="400">
</a>

Note the front and back of the PCB

<a href="images/OLED_Conn_A.jpg">
<img src="images/OLED_Conn_A.jpg" width="400">
</a>
<a href="images/OLED_Conn_B.jpg">
<img src="images/OLED_Conn_B.jpg" width="400">
</a>

Insert the 4 pin connector to the back of the PCB. Align it with the marking on the PCB and then solder each pin from the front.

### **Be sure to solder correctly in this step, as there will be no access to the solder joints once the OLED screen is in place.**

<a href="images/OLEDScreen_A.jpg">
<img src="images/OLEDScreen_A.jpg" width="400">
</a>
<a href="images/OLEDScreen_B.jpg">
<img src="images/OLEDScreen_B.jpg" width="400">
</a>

Insert the short pins of the OLED screen header through the back of the OLED PCB then solder from the front. Then place the long pins of the screen header through the black mounting PCB and solder each pin from the underside.

<a href="images/OLED_Trim_A.jpg">
<img src="images/OLED_Trim_A.jpg" width="400">
</a>
<a href="images/OLED_Trim_B.jpg">
<img src="images/OLED_Trim_B.jpg" width="400">
</a>

Trim header pins short on both side. 

<a href="images/OLED_Trim_C.jpg">
<img src="images/OLED_Trim_C.jpg" width="400">
</a>
<a href="images/OLED_Tilt.jpg">
<img src="images/OLED_Tilt.jpg" width="400">
</a>

Be sure the pins on the front are not protruding higher than the screen. Also, tilt-up the OLED screen slightly. Otherwise, there will be a gap between the case and the screen.

<a href="images/OLED_Install_A.jpg">
<img src="images/OLED_Install_A.jpg" width="400">
</a>
<a href="images/OLED_Install_B.jpg">
<img src="images/OLED_Install_B.jpg" width="400">
</a>

Attached the OLED screen to the left case with 2 M3 5mm screws.

---

## **Mount PCB assembly to case**

<a href="images/Asm_mount_R.jpg">
<img src="images/Asm_mount_R.jpg" width="400">
</a>
<a href="images/Asm_mount_L.jpg">
<img src="images/Asm_mount_L.jpg" width="400">
</a>

There are 5 mounting points on both side. Secure the PCB with the M3 5mm screws.

---

## **Connecting OLED screen**

<a href="images/ConnectOLED.jpg">
<img src="images/ConnectOLED.jpg" width="400">
</a>

Connect OLED screen with the 4 pin cable.


## **Case Assembly**

<a href="images/Case_asm_A.jpg">
<img src="images/Case_asm_A.jpg" width="400">
</a>

Place the side panel onto the case.

**Default Cover**

<a href="images/Case_asm_default.jpg">
<img src="images/Case_asm_default.jpg" width="400">
</a>

Stack default cover onto the case with side panal, then fasten it with 5mm and 16mm screws.

**With tenting risers**

<a href="images/Case_asm_tented.jpg">
<img src="images/Case_asm_tented.jpg" width="400">
</a>

Stack the raiser and default cover onto the case with side panal, then fasten it with 16mm and 25mm screws.

---

<a href="images/Done.jpg">
<img src="images/Done.jpg" width="600">
</a>

---
