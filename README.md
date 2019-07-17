## Adafruit GPIO Expander Bonnet PCB

<a href="http://www.adafruit.com/products/4132"><img src="assets/4132.jpg?raw=true" width="500px"><br/>
Click here to purchase one from the Adafruit shop</a>

PCB files for the Adafruit GPIO Expander Bonnet. Format is EagleCAD schematic and board layout
* https://www.adafruit.com/product/4132

### Description

The Raspberry Pi is an amazing single board computer - and one of the best parts is that GPIO connector! 40 pins of digital goodness you can twiddle to control LEDs, sensors, buttons, radios, displays - just about any device you can imagine. This Adafruit GPIO Expander Bonnet will give you even more digital deliciousness - 16 more digital input/output pins are yours for any desire you have. The outputs are grouped into two 16-pin connectors that have a matching ground pin. You can set each pin to be a digital output (high or low) or as an input, with an internal pull-up if you like!

Simply pop the Bonnet on top of your Pi, the circuitry connects to the SDA/SCL I2C pins for control. The MCP23017 chip converts our Python commands to pin instructions.

When used as an output, each pin can supply up to 20mA (current clamped) - so you can drive LEDs directly. The datasheet recommends you keep the total current draw to under 125mA for the whole chip. We set up the expander chip for 5V logic by default (the I2C is level shifted so that's 3V logic). We did that so you can drive white, blue or green LEDs that sometimes aren't too happy with 3.3V logic. Or, you can cut/solder a jumper to change it to 3.3V logic.

When used as an input, you can set up a pull-up resistor so buttons and switches don't need extra resistors - just wire the pin to one side and ground to the other! There's interrupt capabilities on the chip, and two IRQ pins (INTA and INTB) you can solder a wire to, if you want to have a quick way of telling if any of the GPIO's changed.

By soldering close the address select jumpers, you can change the address from 0x20 up to 0x27. So, if you wanted to, you could have up to 8 bonnets for 128 total GPIO.

Comes as an assembled and tested Bonnet with slim 2x20 header connector on the bottom. We provide 2 sets of 16-pin IDC sockets, you can solder these in or leave them off for a slim setup. [Follow our guide to use our CircuitPython library with Python 3 for fast and easy setup and configuration, you'll be running in under 5 minutes.](https://learn.adafruit.com/gpio-expander-bonnet/overview)

### License

Adafruit invests time and resources providing this open source design, please support Adafruit and open-source hardware by purchasing products from [Adafruit](https://www.adafruit.com)!

Designed by Limor Fried/Ladyada for Adafruit Industries.

Creative Commons Attribution/Share-Alike, all text above must be included in any redistribution. See license.txt for additional details.
