# usb-sound
USB sound card for ham radio

## Features
 - Adjustable input attenuation (for mic in and left channel)
 - Configurable OMTP jack (TRRS; left, right, mic, gnd)
 - PTT circuit (pulls down to gnd)
 - (Optional) Mini-DIN8 Port compatible with Xiegu transceivers (designed for the G90)
 - CM108B IC

## Technical Details
There is a massive test point (marked "PTT") so you can solder whatever you want to control on.
> [!NOTE]
> The PTT pin is shorted to GND when activated, with no current limiting or decoupling.
There are two audio jacks. By default, they are configured as:
 - OUT: T=Left out, S=GND
 - IN: T=Input, S=GND
The OUT jack is configurable (through two solder jumpers on the back) for an OMTP style:
 - T=Left out
 - R1=Right out
 - R2=Mic in
 - S=GND
There are two 10k potentiometers configured as voltage dividers to attenuate the left channel and the mic input.
They each have a 1k resistor connected from wiper to ground to make them feel more logarithmic.
Additionally, there is an additional 10k resistor in series of each potentiometer to attenuate the signal more.
