To burn the firmware (no bootloader):

	avrdude -c usbtiny -p t85 -U flash:w:main.hex -U lfuse:w:0xe1:m -U hfuse:w:0xdd:m

This will leave the reset pin active, so you can change the firmware later on.
