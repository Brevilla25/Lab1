# Lab1

#Part 2 - Flashing & Debugging Code 
1. As the code begins to The LD 4 on the STM32 flashes green and red and creates new folders, a debugging window on the right is opened up where you can add variable expressions to watch. A debug folder is made. To look at what part of memory is written to on the MCU you can look at the map file, under the "Linker script and memory map" section. A USB cord is used to connect/communicate to your STM32 board from your computer, we also had to install USB drivers when installing the application to recongnize this specific USB connection, and the communcation/connection updates are outputted in the console. To transfer a compiled binary to the STM32 microcontroller, you use a combination of a hardware tool (ST-LINK or J-Link) aka a programmer or debugger, a software tool, and an underlying communication protocol (SWD or JTAG)


#Part 3 - Blinking LEDS

 There are three USER LEDS, LD1-3. These are connected to the MCUs GPIO pins which lets us turn them off or on using software. They are memory-mapped, so the MCU can read them as if they are a memory address. Pin names: PC7 (green), PB7 (blue), PB14(red). The pins are configured as GPIO's, that means means setting a pin on a microcontroller (STM32) or processor to act as a programmable digital signal line rather than a fixed hardware function. They should be configured as output because we want the pin to actively drives an electrical voltage outward to control an external component (aka turning an LED on/off).

## Video

[Watch or download IMG_3378.MOV](3-blink/IMG_3378.MOV)