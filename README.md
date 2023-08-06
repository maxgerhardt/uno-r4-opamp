# Arduino Uno R4 OPAMP Example

## Description

The Uno R4 WiFi features an internal OMAMP in its Renesas RA4M1 series microcontroller.

The Operational Amplifier has a Plus and Minus (non-inverting, inverting) input and an output. 

See https://www.allaboutcircuits.com/video-tutorials/op-amp-applications-voltage-follower/
for a simple setup for an OpAmp in the configuration of a "voltage follower": If Minus and Output are connected, the output will
follow (mirror) the voltage applied to Plus with respect to GND, within the electrical limits of the OpAmp.

You can also build small amplifiers with this etc.

## Pinout

Pinout on Uno R4 WiFi:
* A1 is OMAMP PLUS (+)
* A2 is OMAMP MINUS (-)
* A3 is OMAMP OUTPUT (O)

## Example Test

Upload the sketch to the Uno R4 WiFi. Connect A2 and A3 to the same row in a breadboard (connected together).

Connect A1 to GND. You should see that the voltage on A2/A3 in regards to GND is now also GND.

Connect A2 to 3.3V. You should see that the voltage on A2/A3 in regards to GND is now also 3.3V.

## References

See schematics at https://docs.arduino.cc/hardware/uno-r4-wifi

See documentation https://renesas.github.io/fsp/group___o_p_a_m_p.html

Search "Renesas RA4M1 Group User’s Manual: Hardware"

Search "Renesas RA4M1 Group Datasheet"
