# blink
### 12/29/2025 - MM/DD/2025

See LOG.md for daily logs.

## Abstract
- This project is comprised of multiple parts
- __Part One__: the board's green LED will toggle on and off in 500 ms intervals
- __Part Two__: the board's green LED will stay lit, but can be toggled to various brightness levels using the board's user button
- Will use the STM32's general purpose timers rather than HAL_Delay()
- Polling is utilized rather than interrupts

## What I learned
- Initializing and utilizing the STM32's general purpose timers
- Polling a status register
- Using pulse width modulation to dim the brightness of an LED

## Issues
- 

__Comments__
- 