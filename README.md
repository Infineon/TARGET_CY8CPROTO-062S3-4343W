# CY8CPROTO-062S3-4343W BSP

## Overview

The CY8CPROTO-062S3-4343W Kit is a low-cost hardware platform that enables design and debug of the PSoC 62 MCU (CY8C6245LQI-S3D72) and the Murata LBEE5KL1DX Module (CYW4343W WiFi + Bluetooth Combo Chip).
![](docs/html/board.png)

To use code from the BSP, simply include a reference to `cybsp.h`.

## Features

### Kit Features:

* Support of up to 512 KB Flash and 256 KB SRAM
* Dedicated SDHC to interface with WICED wireless devices.
* Delivers dual-cores, with a 150-MHz Arm Cortex-M4 as the primary application processor and a 100-MHz Arm Cortex-M0+ as the secondary processor for low-power operations.
* Supports Full-Speed USB, capacitive-sensing with CapSense.

### Kit Contents:

* CY8CPROTO-062S3-4343W board
* USB Type-A to Micro-B cable
* Quick Start Guide

## BSP Configuration

The BSP has a few hooks that allow its behavior to be configured. Some of these items are enabled by default while others must be explicitly enabled. Items enabled by default are specified in the CY8CPROTO-062S3-4343W.mk file. The items that are enabled can be changed by creating a custom BSP or by editing the application makefile.

Components:
    * Device specific HAL reference (e.g.: PSOC6HAL) - This component, enabled by default, pulls in the version of the HAL that is applicable for this board.
    * CYBSP_WIFI_CAPABLE - This component, disabled by default, causes the BSP to initialize the interface to an onboard wireless chip.
    * BSP_DESIGN_MODUS - This component, enabled by default, causes the Configurator generated code for this specific BSP to be included. This should not be used at the same time as the CUSTOM_DESIGN_MODUS component.
    * CUSTOM_DESIGN_MODUS - This component, disabled by default, causes the Configurator generated code from the application to be included. This assumes that the application provides configurator generated code. This should not be used at the same time as the BSP_DESIGN_MODUS component.

Defines:
    * CY_USING_HAL - This define, enabled by default, specifies that the HAL is intended to be used by the application. This will cause the BSP to include the applicable header file and to initialize the system level drivers.

### Clock Configuration

| Clock    | Source    | Output Frequency |
|----------|-----------|------------------|
| CLK_HF0  | CLK_PATH0 | 100 MHz          |
| CLK_HF2  | CLK_PATH0 | 50 MHz           |
| CLK_HF3  | CLK_PATH1 | 48 MHz           |
| CLK_HF4  | CLK_PATH0 | 100 MHz          |

### Power Configuration

* System Active Power Mode: LP
* System Idle Power Mode: Deep Sleep
* VDDA Voltage: 3300 mV
* VDDD Voltage: 3300 mV

## API Reference Manual

The CY8CPROTO-062S3-4343W Board Support Package provides a set of APIs to configure, initialize and use the board resources.

See the [BSP API Reference Manual][api] for the complete list of the provided interfaces.

## More information
* [CY8CPROTO-062S3-4343W BSP API Reference Manual][api]
* [CY8CPROTO-062S3-4343W Documentation](www.cypress.com/documentation/development-kitsboards)
* [Cypress Semiconductor](http://www.cypress.com)
* [Cypress Semiconductor GitHub](https://github.com/cypresssemiconductorco)
* [ModusToolbox](https://www.cypress.com/products/modustoolbox-software-environment)

[api]: https://cypresssemiconductorco.github.io/TARGET_CY8CPROTO-062S3-4343W/html/modules.html

---
© Cypress Semiconductor Corporation, 2019-2020.