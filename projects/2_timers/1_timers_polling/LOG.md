# Daily Logs


### 01/02/2025

__Activity__
- Initialized the red, green, and blue LED pins (GPIOB)
- Using the RCC register, enabled TIM2 and the clocks for GPIOB (LEDs) and GPIOC (user button)
- Configured GPIO pins (input or output, pull-up or pull-down, etc)

__Issues__
- None

__Possible Solutions and Next Steps__
- N/A

__Comments__
- Nothing's gone wrong so far
  - But nothing __can__ go wrong so far...
___


### 01/04/2025

__Activity__
- Configured the control registers (CR1 and CR2) for TIM2
- Found the relevant clock source and frequency
- Calculated and loaded the appropriate prescaler value into the relevant register
- Wrote the code to make the green LED blink

__Issues__
- The LED blinks too quickly D:

__Possible Solutions and Next Steps__
- Recalculate prescaler value
- Double check clock source and frequency

__Comments__
- It's ok! Should be an easy fix
___


### 01/09/2025

__Activity__
- Recalculated prescaler value and loaded it into the relevant register
- Wrote the code to change the active LED and keep the selected LED on until the user button is released

__Issues__
- The green LED stays off while the button is held down (incorrect!)
  - The red and blue stay on (correct!)

__Possible Solutions and Next Steps__
- An unsigned char is used to track which LED is active
  - When the user switches to the green LED, an if statement is entered to wrap the char around
  - Maybe that is messing with something

__Comments__
- Huh.
___