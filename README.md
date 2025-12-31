# stm32_DMA
This project demonstrates bare-metal programming of the STM32F401CC using ADC with DMA, timer-triggered sampling, and UART transmission in Proteus.

# Features
- Internal HSI 16 MHz clock (no external crystal)
- TIM2 triggers ADC at 100 Hz
- ADC1 + DMA captures analog input (PA0)
- USART2 @ 57600 baud outputs data (PA2)

# Proteus Setup
- Connect PA2 (TX) → Virtual Terminal RXD
- Connect GND → GND
- Virtual Terminal: 57600, 8-N-1

# Build & Run
- Create an STM32CubeIDE empty project for STM32F401CC
- Replace main.c with the provided source
- Build the project
- Load the generated .elf file into Proteus
- Run simulation and observe UART output

# Notes
- external oscillator not required
- Designed specifically for Proteus simulation
