# Parts

## Bill of materials

| Qty | Part | Role |
| --- | --- | --- |
| 1 | Raspberry Pi Pico 2 (with header) | the node |
| 1 | Raspberry Pi Pico Debug Probe | SWD flash and debug, UART0 console |
| 2 | USB A to USB Micro-B cable | one for the Pico, one for the Debug Probe |
| 1 | Full-size breadboard | assembly |
| 1 | Jumper wire set (M-M, M-F, F-F) | assembly |
| 1 | 1602 LCD with PCF8574 I2C backpack | local menu display |
| 1 | VS1838B infrared receiver | menu navigation input |
| 1 | NEC-compatible infrared remote | menu navigation input |
| 3 | 5 mm LEDs (red, yellow, green) | menu position indicator |
| 3 | 220 or 330 ohm resistors | LED current limit |
| 2 | RYLR998 LoRa module | one on the node, one on the gateway |

## Roles

- Node: Pico 2 plus every peripheral above except the second RYLR998.
- Gateway: the computer with the second RYLR998 on a USB serial adapter.
- Debug Probe: flashing, SWD debugging, and the UART0 console.

## Notes

- The infrared receiver idles high and pulses low on an active mark.
- The LCD backpack address is 0x27.
- The menu holds three items: START, SET, and INFO.
