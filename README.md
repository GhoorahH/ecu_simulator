
# ECU Simulator – STM32F446RE

## Project Overview
Short description...

## Architecture
Timer-based scheduler...

## Hardware
- STM32 NUCLEO-F446RE
- MCP2562 CAN transceiver
- 10k potentiometer

## Step 1 – Real-Time Scheduler
System Clock (84 MHz)-> TIM2 Timer -> (every 10ms) Timer Interrupt -> ECU_10ms_Task()

- Timer used: TIM2
- Timer period: 10 ms
- Interrupt mode: Enabled (NVIC)
- Callback function: HAL_TIM_PeriodElapsedCallback()

