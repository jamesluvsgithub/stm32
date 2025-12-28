# blink
### 12/23/2025 - MM/DD/YYYY

__Abstract__
- This is a simple blink project using the STM32's HAL calls
- The board's green LED will toggle on and off in 500 ms intervals

__What I learned__
- How to generate code in STM32CudeIDE by configuring the .ioc
- Using basic HAL functions, like HAL_GPIO_TogglePin()
- The process of building and runnning a project

__Issues__
- The LED seemingly refused to blink, even after:
    - Moving initialization steps to many different functions
    - A lot of time trying different at Run configurations
    - Manually writing 1 and 0 to the pin with WritePin() rather than using TogglePin()
    - Unplugging and replugging the board to cause a reset

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
- Analyze the initialization stage of my code; the main loop (two lines of code) seems to check out..

__Comments__
- Oh no
___



### 12/26/2025

__Activity__
- Moved GPIOB initialization from main function to MX_GPIO_Init()
- Manually wrote 1 and 0 to the pin with WritePin() rather than using TogglePin()

__Issues__
- LED still does not blink...

__Possible Solutions and Next Steps__
- Read more documentation or watch more Youtube videos on how to initialize a port pin
- Check debug/run and build configurations. Perhaps the board isn't even receiving the code somehow..?
- Move initialization somewhere else? Maybe my configurations are being overwritten somehow?????

__Comments__
- Aw rats
___



### 12/28/2025

__Activity__
- I did it. I finally did it.
- After running the program in debug mode, I found that the program reached MX_ETH_Init() and then stopped.
- Commenting out the function and resetting allowed the LED to blink

__Issues__
- NONE

__Possible Solutions and Next Steps__
- Investigate MX_ETH_Init() and find out why it breaks the program

__Comments__
- Yay!! Still have some work to do though...
___
