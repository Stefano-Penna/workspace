# Workspace
Embedded software development workspace for microcontrollers.

## Supported targets:
- LPC1769
- LPC4337 (M4 and M0 cores)

## Supported boards:
- CIAA-NXP and EDU-CIAA-NXP (www.proyecto-ciaa.com.ar)
- LPCXpresso with LPC1769

## Available libraries:
- [CMSIS](http://www.arm.com/products/processors/cortex-m/cortex-microcontroller-software-interface-standard.php) and [LPCOpen](https://www.lpcware.com/lpcopen)
- [CMSIS-DSPLIB](http://www.keil.com/pack/doc/CMSIS/DSP/html/index.html)
- [lwip](http://lwip.wikia.com/wiki/LwIP_Wiki)
- [FreeRTOS](http://www.freertos.org/)

## Supported toolchains:
- gcc-arm-none-eabi

## Usage
* Make sure you have an ```arm-none-eabi-*``` toolchain configured in your ```PATH```.
* ```git clone https://github.com/pridolfi/workspace.git && cd workspace```
* ```cp project.mk.template project.mk```
* Define ```PROJECT```, ```TARGET``` and ```BOARD``` (optional) variables in ```project.mk``` according to the project you want to compile.
* Compile with ```make```.
* Clean with ```make clean```.
* Download to target via OpenOCD with ```make download```.
