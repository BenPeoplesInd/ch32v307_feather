# ch32v307_feather
Feather-ish board for ch32v307rct6

This is a rough pass at a ch32v307 feather using the 64-pin variant of the CH32V307.   

At this moment it's untested (I'm ordering them now).    USB-C for the programming adapter.

A few notes vs. the official feather:

- I've omitted the LiPo stack
- Current vreg is only 100mA
- BOOT button connects BOOT0 to 3.3V to enable bootloader over USB
- There's no debug via USB (unless you write one)
- No SWD breakout
- Includes 5.1k resistors for USB-C PD
- All the GPIOs are ADC capable
- Did not breakout the ethernet pins anywhere, which might actually be super useful.  
- No status/indicator LEDs
- SPI is SPI2
- i2c is also USB2
- Schematic is messy and poorly documented
