# blink
### 12/29/2025 - MM/DD/2025

See LOG.md for daily logs.

## Abstract
- This project is comprised of multiple parts
- __Part One__: An LED on the board will toggle on and off in 500 ms intervals, defaulting to the green LED. The user button can be pressed to switch the current active LED. The newly active LED will remain lit until the button is released. Polling will be utilized rather than interrupts.
- __Part Two__: The same as part one, but will utilize interrupts instead of polling
- Will use the STM32's general purpose timers rather than HAL_Delay()

## What I learned
- Initializing and utilizing the STM32's general purpose timers
- Calculating delay time in seconds based on clock frequency and prescaler
- Polling a status register

## Issues
- The LEDs blinked too quickly at first

__Comments__
- This was fun! And not as hair pulling as the blink project somehow...