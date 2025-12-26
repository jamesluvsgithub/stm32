# blink
### 12/23/2025 - MM/DD/YYYY

__Abstract__
- This is a simple blink project using the STM32's HAL calls
- Applications of the project

__Issues__
- Any problems encountered

__What I learned__
- How to generate code in STM32CudeIDE by configuring the .ioc
- Using basic HAL functions, like HAL_GPIO_TogglePin()

__Comments__
- This was... harder than expected..
___



## Daily Logs


### 12/23/2025

__Activity__
- Read about HAL functions
- Initialized GPIOB Pin 7 (Green LD2) by generating code
- Toggled GPIOB Pin 7, followed by a 500 ms delay

__Issues__
- LED does not blink...

__Possible Solutions and Next Steps__
- Analyze the initialization stage of my code

__Comments__
- Oh no
___



### 12/26/2025

__Activity__
- Moved GPIOB initialization from main function to MX_GPIO_Init()

__Issues__
- LED still does not blink...

__Possible Solutions and Next Steps__
- Read more documentation or watch more Youtube videos on how to initialize a port pin

__Comments__
- Aw rats
___
