# Hardware

The intended hardware platform for this project is the Raspberry Pi Pico 2.

## Measurements

### Temperature

Plant buddy should be capable to measure the soil and air temperature of a
plant. In addition it should be somehow extensible to add additional temperature
sensors. Since the intention is to measure in the plant compatible temperature
range i'd eyeball the range to be something between -30 °C to 80 °C with a
resolution and accuracy of ~ 0.1 °C.

[ ] List options for sensors
[ ] Decide on sensor type
[ ] Come up with initial idea for the measurement circuitry
[ ] Come up with a concept of calibration

### Moisture

tbd. probably some capacitive method.

### Light exposure

tbd. maybe an LDR ore something similar

## Data Storage

tbd. maybe an SD card or some other form of flash memory

## Display

tbd. Probably a e-ink display to reduce power consumption

## Power Supply

tbd. probably a system that supports some form of wired power supply, a battery
solution and maybe some solar capabilities. not clear yet.

## Communication

tbd.

Bluetooth or wifi would be maybe nice.
maybe LoRa or Zigbee or what not

### Security

Use the ARM trust zone to somehow store private information. Also if possible
somehow generate an asymmetric key on the device that can be used to store more
secure information in the flash in an encrypted fashion so that it cannot be
read by outsiders. Also somehow add some for of trust for the firmware like
secure boot or something similar.

Explore the possibilities to use elliptic curve algorithms to make better use of
the 8k OTP on the Pico 2.
