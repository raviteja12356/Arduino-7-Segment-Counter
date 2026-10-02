# Arduino-7-Segment-Counter
Arduino-based 0–9 digital counter using a 7-segment display and push button, demonstrating GPIO control, digital input/output, and embedded programming

# Arduino 7-Segment Display Counter

## Description

This project implements a **0–9 counter using an Arduino, a 7-segment display, and a push button**.

Each time the push button is pressed, the displayed number increases by one. After displaying `9`, the counter returns to `0`.

## Components Required

* Arduino Uno
* 7-Segment Display
* Push Button
* 220Ω Resistors
* Breadboard
* Jumper Wires

## Pin Connections

| Segment     | Arduino Pin |
| ----------- | ----------: |
| A           |          10 |
| B           |          11 |
| C           |           7 |
| D           |           8 |
| E           |           9 |
| F           |          13 |
| G           |          12 |
| DP          |           6 |
| Push Button |           4 |

The push button uses the Arduino's internal `INPUT_PULLUP` resistor.

## Working

1. The Arduino initializes all 7-segment display pins as outputs.
2. The push button is configured using `INPUT_PULLUP`.
3. Initially, the display is turned OFF.
4. When the button changes from `HIGH` to `LOW`, the counter is incremented.
5. The counter displays numbers from `0` to `9`.
6. After `9`, the counter starts again from `0`.

## Technologies Used

* Arduino
* Arduino IDE
* Embedded C / Arduino C++
* Digital GPIO
* 7-Segment Display

## Project Output

```text
Button Press
     ↓
    0 → 1 → 2 → 3 → 4 → 5 → 6 → 7 → 8 → 9
     ↑________________________________________|
```

## Author

**KOCHERLA RAVITEJA**

Aspiring Embedded Systems Engineer
