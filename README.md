# Day 2: Button-Controlled LED

This project uses an ESP32 push-button to toggle an external LED. It uses the internal pull-up resistor and software debouncing to prevent one press from registering multiple times.

## Components

- ESP32 DevKit v1
- Push-button
- LED
- 220 Ω resistor

## Connections

- Push-button contact 1 → ESP32 GPIO 4
- Push-button contact 2 → ESP32 GND
- ESP32 GPIO 18 → 220 Ω resistor → LED long leg (anode)
- LED short leg (cathode) → ESP32 GND

Configure GPIO 4 as `INPUT_PULLUP`. The pin reads `HIGH` when the button is released and `LOW` when pressed.

## Wokwi Simulation

[Run the simulation](https://wokwi.com/projects/476323502821270529)

## How to use

1. Start the Wokwi simulation.
2. Press the button once to turn the LED on.
3. Press it again to turn the LED off.

