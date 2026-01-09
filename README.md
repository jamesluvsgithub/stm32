# stm32

The board used is the Nucleo-144 F439ZI. I decided to take a bare-metal approach, manipulating registers directly for things like GPIO, ADC, and DMA.
I only use HAL for system clock configuration.

Each project builds on the last, and they are numbered in order. They all contain the necessary files to build and run the project in a new, blank STM32CubeIDE environment. Every project will contain:
- The source code that I wrote. It will be located in /Core/Src/
- A README.md, which describes:
  - What the project is
  - What I achieved
  - What I learned from the project
  - Any issues I came across
  - Any personal (and informal) comments I have about the project
- A LOG.md, where I log my progress on the project every day that I work on it
- Projects may contain multiple parts. In this case, each part will contain its own folder and LOG.md

I used Mitch Davis's Youtube tutorials extensively to get started. I highly recommend it for beginners such as myself.
