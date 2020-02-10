### CY8CPROTO-062S3-4343W BSP
The CY8CPROTO-062S3-4343W Kit is a low-cost hardware platform that enables design and debug of the PSoC 62 MCU (CY8C6245LQI-S3D72) and the Murata LBEE5KL1DX Module (CYW4343W WiFi + Bluetooth Combo Chip).

### What's New In This Release?
* This release adds updated linker scripts and startup code for the CM0+ and CM4 cores. The files are now in core specific directories.
* Minor updates up avoid potential warnings on some toolchains

### What's Included?
The CY8CPROTO-062S3-4343W library includes the following:
* BSP specific makefile to configure the build process for the board
* cybsp.c/h files to initialize the board and any system peripherals
* cybsp_types.h file describing basic board setup
* CM4 Linker script & startup code for GCC, IAR, ARM toolchains
* CM0+ Linker script & startup code for GCC, IAR, ARM toolchains
* Configurator design files (and generated code) to setup board specific peripherals
* .lib file references for all dependent libraries
* API documentation

### Supported Software and Tools
This version of the CY8CPROTO-062S3-4343W BSP was validated for compatibility with the following Software and Tools:

| Software and Tools                        | Version |
| :---                                      | :----:  |
| ModusToolbox Software Environment         | 2.0     |
| GCC Compiler                              | 7.4     |
| IAR Compiler                              | 8.32    |
| ARM Compiler                              | 6.11    |

### More information
* [CY8CPROTO-062S3-4343W BSP API Reference Manual][api]
* [CY8CPROTO-062S3-4343W Documentation](www.cypress.com/documentation/development-kitsboards)
* [Cypress Semiconductor](http://www.cypress.com)
* [Cypress Semiconductor GitHub](https://github.com/cypresssemiconductorco)
* [ModusToolbox](https://www.cypress.com/products/modustoolbox-software-environment)

[api]: modules.html

---
© Cypress Semiconductor Corporation, 2019.