# blink
### 12/23/2025 - 12/28/2025

See LOG.md for daily logs.

__Abstract__
- This is a simple blink project using the STM32's HAL calls
- The board's blue LED will toggle on and off in 500 ms intervals

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
