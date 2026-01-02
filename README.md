# STM32F103C8T6_UART_Control_28BYJ48
Use UART to control 28BYJ-48 stepper motor speed based on STM32 HAL
# STM32 UART Control 28BYJ-48 Stepper Motor

This project demonstrates how to control the speed of a 28BYJ-48 stepper motor
using UART commands on STM32F103C8T6 with HAL library.

## Hardware
- STM32F103C8T6 (Blue Pill)
- 28BYJ-48 Stepper Motor
- ULN2003 Driver Board
- External 5V Power Supply

## Features
- UART interrupt reception
- Timer (TIM2) interrupt based motor control
- Half-step driving mode
- Speed control via UART commands

## UART Commands
| Command | Description |
|--------|-------------|
| `1` | Slow speed |
| `2` | Medium speed |
| `3` | Fast speed |

## Pin Connection
| ULN2003 | STM32 |
|--------|-------|
| IN1 | PA0 |
| IN2 | PA1 |
| IN3 | PA2 |
| IN4 | PA3 |
| GND | GND |
| VCC | 5V (External) |

## Development Environment
- STM32CubeMX
- STM32CubeIDE
- HAL Library

## Notes
- The motor is driven by TIM2 interrupt, no blocking delay is used.
- UART reception is handled by interrupt.
- This project is part of my STM32 learning practice.

## Author
Y
