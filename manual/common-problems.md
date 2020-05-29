# Common Problems

This file should discuss common problems with the OSCar, and how to deal with them.

## Lost Memory

**Symptoms:** The OSCar appears completely dead, no sound, no lights. 
Turning it off and on again repeatedly may get som LED's lighting up but they will not blink, and there is no sound.

**Cause:** If the synthesizer has been unusued for a long time it's backup battery will drain, and it will lose the memory.
This will also happen when servicing if the CPU board is separated from the control board, 
as it's the control board that houses the battery.

**Solution:** Keep the synthesizer on for several hours to charge the battery. Send a memory dump to it over MIDI, or load from a casette. If this happens repeatedly, then the battery is dead and needs replacing. 


## Dead battery

**Symptoms:** Same as for lost memory, but persistent. It either does not boot even after the battery has charged for hours, or it works temporarily, but loses memory again after one or a few days.

**Cause:** The battery has gone old and doesn't retain a charge.

**Solution:** Replace the battery on the control board.


## Ground loop hum

**Symptoms:** When connecting to some equipment, but not all, the OSCar will cause a significant groulnd loop hum or buzz.

**Cause:** The OSCar has the 0V connected to the Chassi ground, making it prone to creating ground loops.

**Solution:** Put in a low capacitance, low voltage non polar capacitor between the incoming ground and the 0V of the circuit board. For example a 16V 10pF plastic film capacitor. It should be low voltage, you want it to burn up if there is a high voltage over it.


## Corroded circuit board connectors or sockets

**Symptoms:** Glitching and weird behavior, especially while gently pressing on the cover.

**Cause:** Corroded connections, either the connectors between circuit boards, or the IC sockets.

**Solution:** Search out where exactly the problem lies after taking off the plastic cover, 
clean those connectors with contact cleaner. In bad cases you may need to replace them.


## Reset circuitry issues

**Symptoms:** Even after switching batteries the OSCar will start unreliably.

**Cause:** The reset circuitry will tell the processor to start even though the voltage hasn't stabilized yet.

**Solution:** There is no verified good solution for this problem yet.
