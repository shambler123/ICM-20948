## A King is born
# FOC / KING

## The DIY Open Source Vesc6 and FOC capable HW

**01.03.24: VERY CLOSE TO A RELEASE - JUST NEED A FINAL TEST ON UART.
CURRENT PRICE TAG AT JLCPCB FOR 5 BOARDS WITH ALL COMPONENTS ASSEMBLED (not including FETS and Power Capacitors):
  $134.61**

The FOCKING is an open-source motor controller board in development based on a JLCPCB friendly [VESC6 75V/300A](https://vesc-project.com/sites/default/files/Benjamin%20Posts/vesc_75_300.pdf) so-called "driverless" design with individual gate drivers for all three phases. It is powered by an STM32F405 CPU and is capable of running Field Oriented Control at high power and voltages.

FOC is short of Field Oriented Control and KING is because it's the King. The hardware is separated in 3 sub-modules: Power, STM32F405 FOCPILL, and the main module with FOC related components. The board is intended for "small" electric vehicles like Skateboards, OneWheels, Bicycles, Robotics, Boats, and is designed in sub-modules as a reference design for further development.

## Features
* 75V/150A continuous rating
* 18s battery voltage rating
* 3-phase FOC motor control
* 4-layer smd design with individual gate drivers for all three phases
* STM32F405 MCU
* USB-C
* CAN
* Onboard IMU
* 12V AUX Power (for e.g. light or ?)
* Compact design with fets and shunts mounted on the bottom side
* 12V for gate drivers, 5V for CAN and IMU, and 3.3V for MCU and op-amped current-sense amplification
* Cheap and up-to-date with cheapest and **well stocked** components available for ordering at [JLCPCB](https://jlcpcb.com/) and [LCSC](https://www.lcsc.com)

<div>
<img src="f.png"  width="275" height="404" style="float:left; margin-right:10px;">
<img src="b.png"  width="275" height="404" style="float:left;">
</div>

## Getting Started
Prerequisites
To use The FOCKING, you will need the following:

* To wait for the Official Realease announcement
* A brushless motor
* A power source capable of supplying up to 75V and 150A. Minimum voltage is 16V
* A USB-C cable to connect to a computer for programming and configuration
* Motor control software, such as the VESC firmware

## Installation
To install the FOCKING board, follow these steps:

* Order the PCB from JLCPCB using the provided gerber files
* JLCPCB can offer the service of mounting all components, with the exception of shunts and mosfets
* Purchase the necessary components (BOM available in the repository)
* Solder the remaining components onto the PCB
* Program the firmware onto the board using a programmer (JTAG or Stm32f4Discovery)
* Connect the motor, power source, and USB cable

## Usage
After installation, use the VESC Tool to configure the motor controller according to your specific motor and application requirements.

## Contributions
Contributions to The KING project are welcome and encouraged. If you have any suggestions or improvements, please open an issue or a pull request on the GitHub repository.

## Donate
If you find this project useful and would like to support bread-and-butter for very time consuming development and maintenance, you can [donate 1$](https://www.paypal.com/donate/?business=R5QUC7RNEPKDC&no_recurring=0&item_name=A+small+but+important+contribution+for+Development+and+Maintenance.+Thank+You+very+much.&currency_code=USD) to the creator via [PayPal](https://www.paypal.com/donate/?business=R5QUC7RNEPKDC&no_recurring=0&item_name=A+small+but+important+contribution+for+Development+and+Maintenance.+Thank+You+very+much.&currency_code=USD).
<img align="right" src="QR-kode.png">


## License
The KING is released under the CERN Open Hardware License (OHL), developed by the European Organization for Nuclear Research. In short, it is a permissive license that allows anyone to use, modify, and distribute the licensed hardware, as long as they provide attribution to the original creators and distribute their modifications under the same license.

## Acknowledgements
The KING is built on the work of the [VESC project](https://github.com/vedderb/bldc) and the contributions of its developers and contributors. Many thanks to *mxlemming* (aka [David Molony](https://github.com/davidmolony/MESC_FOC_ESC)) and *crinq* on the vesc forum on discord for their careful review and advice. Also this project is inspired by the format and concept of the [MP2](https://github.com/badgineer/MP2-ESC) by *badgineer* and the [Cheap Focer2](https://github.com/shamansystems/Cheap-FOCer-2/blob/Developer-Branch/README.md) by *shaman*.
