# MCU Showcase

[![Language](https://img.shields.io/badge/language-C-blue)]()
[![License: MIT](https://img.shields.io/badge/license-MIT-green)](LICENSE)

[English](README.md) | [中文](README.zh-CN.md)

A curated collection of microcontroller (MCU) example projects for learning, quick reference, and rapid prototyping. Covers application-layer demos, RTOS examples, bootloader workflows, and hardware driver implementations.

## Categories

| Category | Description | Examples |
|----------|-------------|----------|
| **app** | Application-layer projects using drivers or RTOS features | LED blinkers, sensor readers, communication demos |
| **rtos** | Real-time OS examples | Task scheduling, queues, semaphores, timers |
| **bootloader** | Firmware upgrade workflows | Serial, USB, and OTA update demos |
| **driver** | Hardware peripheral drivers | GPIO, UART, SPI, I2C, ADC/DAC |

## Supported Platforms

Examples primarily target STM32 (Cortex-M3/M4) but the driver layer and RTOS patterns are portable across Cortex-M devices. Each project specifies its target MCU in its own README.

## Usage

1. Clone the repository:

```bash
git clone https://github.com/iron-lambda/mcu-showcase.git
```

2. Navigate to the project of interest:

```bash
cd mcu-showcase/<category>/<project-name>
```

3. Build and flash using the project-specific toolchain (GCC + Make, Keil MDK, or STM32CubeIDE).

## Prerequisites

- ARM GCC toolchain (`arm-none-eabi-gcc`) for Make-based projects
- [Keil MDK](https://www.keil.com/) for `.uvprojx` projects
- [STM32CubeMX](https://www.st.com/en/development-tools/stm32cubemx.html) (optional, for regenerating HAL code)
- OpenOCD or ST-Link for flashing

## Contributing

Contributions are welcome! To add a new example:

1. Create a directory under the appropriate category (`app/`, `rtos/`, `driver/`, or `bootloader/`)
2. Include a `README.md` explaining the project, target hardware, and build instructions
3. Keep the code self-contained with minimal external dependencies

## License

[MIT](LICENSE)
