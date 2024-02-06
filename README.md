# Expansion Module: Arduino UNO

![Hardware](https://img.shields.io/badge/Hardware-PCB-red)
![Design](https://img.shields.io/badge/Design-Schematic-blue)
![made-with-eagle](https://img.shields.io/badge/Made%20with-Eagle-blue.svg)
![Hardware](https://img.shields.io/badge/Hardware-Expansion%20Module-blue)
![Interface](https://img.shields.io/badge/Interface-UART-yellow)
![license](https://img.shields.io/badge/license-MIT-green)

## Overview
This repository hosts the design and implementation of an expansion module that is fully compatible with Arduino UNO, utilizing a single smartboard connector. This module is specifically designed to facilitate and enhance working with FPGA systems within the smartboard ecosystem. It allows for UART connection to FPGA circuits, and I2C communication with the smartboard's socket bus, enabling easy programming and configuration of other modules requiring I2C setup. Additionally, it supports sending and receiving interrupts to/from the FPGA, streamlining high-level debugging and simplifying hardware project control loaded onto the FPGA matrix.

The module's integration with Arduino's simplicity allows for the rapid addition of software functions for debugging or configuring hardware components, such as cameras, making it an invaluable tool for accelerating and improving work with FPGA systems on smartboards. It offers an efficient way to implement high-level debugging and straightforward project control over the hardware setup.

The module is programmed via a USB port, ensuring easy and accessible firmware updates and configurations. Users are reminded to load the Arduino firmware into the module upon assembly for booting, communication, and programming purposes.

## ATmega32u4 Microcontroller

The core of this expansion module is the ATmega32u4 microcontroller, which brings the advantage of having built-in USB communication, eliminating the need for an external USB-to-serial converter. This microcontroller operates at a frequency of 16 MHz and is equipped with 32KB of flash memory, 2.5KB of SRAM, and 1KB of EEPROM. Its integrated USB functionality not only simplifies programming and communication but also enables the module to act as a USB device itself, such as a mouse, keyboard, or other HID device, opening up a plethora of possibilities for embedded projects.

Key features of the ATmega32u4 include:
- Native USB support, facilitating direct programming and communication without additional hardware.
- 23 general-purpose input/output pins (GPIO), including PWM, analog inputs, and support for I2C and SPI communication.
- Built-in hardware support for serial communication via USART, making it ideal for projects that require communication with other microcontrollers or devices.

This microcontroller's versatility and comprehensive feature set make it an excellent choice for developers looking to leverage Arduino UNO compatibility with enhanced connectivity and processing capability.

For more detailed information on the ATmega32u4 microcontroller, including technical specifications and usage guidelines, please refer to the [ATmega32u4 Datasheet](ATmega16U4-32U4-DTE.pdf) available in this repository.

## Compatibility with Arduino UNO

This expansion module is designed to be fully compatible with the Arduino UNO, one of the most popular and versatile development boards in the Arduino ecosystem. By matching the Arduino UNO pinout, this module allows users to take advantage of the vast array of existing Arduino shields and accessories, thereby expanding the scope of projects and applications without requiring additional hardware modifications.

The compatibility with Arduino UNO enables developers to leverage the extensive Arduino library and IDE for programming the module, making it accessible for beginners and powerful enough for advanced users. This opens up opportunities for a wide range of applications, from simple hobbyist projects to complex, integrated IoT systems.

Key benefits of Arduino UNO compatibility include:
- Access to a wide range of Arduino-compatible shields and modules, enhancing the module's utility and flexibility.
- The ability to use the Arduino IDE for programming, which simplifies development and debugging processes.
- Support for Arduino's vast ecosystem, including libraries, tools, and community resources, which can significantly accelerate development time.

This synergy between the ATmega32u4 microcontroller and the Arduino UNO compatibility ensures that developers can quickly and easily create projects with advanced features and capabilities, while maintaining the simplicity and ease of use that Arduino is known for.

To fully harness the potential of this module in the Arduino environment, ensure that the appropriate Arduino bootloader is installed, allowing for seamless integration and programming via the Arduino IDE.

## Media
- ![Schematic](media/sch.png)
- ![Board Design](media/brd.png)
- ![Module Size](media/brd_size.png)
- ![Smartboard with Arduino UNO](media/smartboard_with_arduino_uno.png)
- ![Smartboard System Example](media/smart_board_1.png)

## Contributions and Feedback
Contributions to this project are welcome. If you have suggestions for improvement or have developed additional features, please fork the repository, make your changes, and submit a pull request. For any questions or issues, please open an issue in the GitHub repository.

## License
This project is licensed under the MIT License with the following terms:

- **Permission to Use**: You are free to use, modify, and distribute this design in both private and commercial settings.
- **Attribution Requirement**: While not required, attribution to the original author, Adam Łuczak, is appreciated. This can be done through a citation or a link back to this repository.
- **No Warranty**: This design is provided "as is", without warranty of any kind. Use it at your own risk.
- **Liability**: The author is not liable for any damages or losses that may arise from the use of this design.

For the full terms and conditions, please refer to the MIT License documentation.

## Contact
Should you have any inquiries or suggestions regarding this project, please don't hesitate to contact Adam Łuczak at adam.luczak@outlook.com.
