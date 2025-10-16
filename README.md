# miniarm-microkernel
A simple microkernel implemented on ARM Cortex-M (Raspberry Pi Pico / RP2040) featuring multitasking scheduling, time slicing, synchronization mechanisms, and sensor interaction.

## Features
- Round-robin task scheduling (time-slice)
  - **Round-Robin** (time-slice)
  - **Priority-based** scheduling
  - **Preemptive** task switching
  - **Cooperative** (yield-based)
- Context switch using SysTick
- Mutex & Semaphore
- Inter-task communication (Queue / IPC)
- Simple timer management
- Hardware demo: LED, Servo, Fan, Sensor tasks

## Hardware

### Microcontroller
- **Raspberry Pi Pico (RP2040)**  
  Dual-core ARM Cortex-M0+ (up to 133 MHz, default 48 MHz), 264 KB SRAM, 2 MB Flash.

### Expansion Board
- **Grove Shield for Pico**  

### Actuator Modules
- **L9110 Fan Module x1**
- **SG90 9G Servo Motor 180° x1**
- **Circus LED Indicator 10mm (Red / Green / Yellow / Blue) x4**
- **Circus Passive Buzzer Module x1**
- **Circus Infrared Emitter Module x1**
- **Circus Pixel RGB LED x4 Module x1**
- **Circus 1.3-inch OLED Display Module x1**

### Sensor Modules
- **Circus Light Sensor Module x1**
- **Circus SHT3x Temperature & Humidity Sensor Module x1**  
- **Circus PIR Motion Detector Module x1**
- **Circus Vibration Sensor Module x1**  
- **Circus Adjustable Potentiometer Module x1**
- **Circus Tactile Button Module x1 (random color)**

## Directory Structure
```
miniarm-microkernel/
│
├── README.md
├── LICENSE
├── Makefile
├── docs/
├── kernel/
├── src/
├── include/
├── tasks/
├── drivers/
├── tests/
└── build/
```