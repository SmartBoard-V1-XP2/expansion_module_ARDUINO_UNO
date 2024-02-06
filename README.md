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


## Key Features of ATmega32u4 Module
- **ATmega32u4 Microcontroller**: Offers native USB support, eliminating the need for an external USB-to-serial converter.
- **Arduino UNO Compatibility**: Pinout and interface are fully compatible with Arduino UNO, making it easy to use with existing shields and projects.
- **Multiple Interfaces**: Includes I2C, SPI, and UART for connecting a wide range of peripherals.
- **Integrated USB**: Facilitates easy programming and communication without additional hardware.
- **Compact Design**: Designed to fit into small projects with limited space while offering full functionality.

For more detailed information on the ATmega32u4 microcontroller, including technical specifications and usage guidelines, please refer to the [ATmega32u4 Datasheet](ATmega16U4-32U4-DTE.pdf) available in this repository.

## Module Overview
The module is engineered for rapid prototyping and development, providing a robust platform for creating sophisticated projects that require USB connectivity and Arduino compatibility. It offers an excellent balance between power and performance, allowing users to take advantage of the ATmega32u4's features in a form factor that is fully compatible with the Arduino UNO ecosystem.

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
