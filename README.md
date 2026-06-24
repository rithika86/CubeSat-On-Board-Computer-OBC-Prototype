# CubeSat On-Board Computer (OBC) Prototype

A FreeRTOS-based CubeSat OBC prototype implemented on the STM32F103C8T6 (Blue Pill).

## Features

BMP280 sensor interfacing via I2C

Periodic telemetry generation

UART command interface

Health monitoring task

Safe mode fault management

Inter-task communication using FreeRTOS queues

System reboot command

## Implemented Tasks

Sensor Task - Acquires BMP280 temperature and pressure data

Telemetry Task - Sends telemetry packets over UART

Command Task - Processes ground commands

Health Task - Monitors system health and detects faults

## Commands

HELP
STATUS
SAFE
NORMAL
REBOOT

## Fault Handling

The OBC automatically enters SAFE MODE when sensor communication fails, the telemetry task becomes unresponsive, or the telemetry queue overflows.

## Hardware

STM32F103C8T6 (Blue Pill)

BMP280 Pressure and Temperature Sensor

USB-to-UART Converter

## Demonstrated

FreeRTOS multitasking

Queue-based inter-task communication

Real-time telemetry generation

Command and control interface

Fault detection and safe mode recovery

Author: Rithika R
