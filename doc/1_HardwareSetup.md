# Getting Started - Hardware Setup
## Materials needed
* 2 hoverboard motor controller boards
* solder / soldering iron / solder pump
* 4 male header pins
* 4 female to female jumper wires
* ST Link V2


## Setting up the board
In the setup, we'll be referencing positions of certain things on the board. To make sure we're all on the same page, let's orient the board such that the heat sink is at the top.

Before we can wire anything up, we'll need to prepare the board by soldering debug pins onto it, marked in the red rounded rectangle below:

![pin locations](pin_locations.png)

1. Place the 4 male header pins into the debug pin holes.
2. Solder the pins into place

## Wiring
To flash the ST, we'll need to connect the debug pins to our ST Link V2 microcontroller. The 4 pins to the left of the ST, from left to right, are:
```
3.3V
GND
SWDIO
SWCLK
```

Depending on what ST Link V2 you have, you'll hook it up differently.
If you have the [10 pin version](https://www.mouser.com/ProductDetail/Adafruit/2548/?qs=SElPoaY2y5K%252bwHNUAvyTvg%3D%3D) that plugs directly into the computer USB port, just match each of the debug pins to however your ST Link V2 is labeled:

|  Motor Board |  ST Link V2  |
|:---:|:---:|
| SWDIO  | SWDIO  |
|  GND |  GND |
| SWCLK  |  SWCLK |
| 3.3V  | 3.3V  |
| reset pin (optional)  |  RST |

