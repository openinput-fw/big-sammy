# big-sammy

[![Documentation Status](https://readthedocs.org/projects/big-sammy/badge/?version=latest)](https://openinput.readthedocs.io/projects/big-sammy/en/latest/?badge=latest)

[<img src="docs/assets/logo.svg" alt="" width="20%" align="right">](https://github.com/openinput-fw)

Open source wired mouse hardware.

## Specifications
- 8 kHz sampling rate support
- Zero latency switch debounce
- Onboard configuration memory
- 2 main mouse buttons (satellite* configuration for both)
- 2 side buttons (symmetric to allow easy left/right handedness)
- encoder + wheel button (satellite* configuration)
- RGB Led

`*meaning, a separate board from the core with the controller and sensor`

## Hardware

<img src="docs/assets/r0.1-core-render.png" alt="" width="50%">

- ATSAMS70 MCU (ATSAMS70JxxB-M)
- Optical sensor [PMW3330, PMW3360, PMW3389, Truemove3]
- onboard conectors:
    - JST PH (2mm pitch) for USB
    - JST SH (1mm pitch) for stellite boards
- M2 mounting hardware

|USB pinout||
|-----|-----|
|1|VCC|
|2|DM|
|3|DP|
|4|GND|
|5|Shield|

Peripheral boards are used for the buttons and encoder, available at [generic-mouse-boards](https://github.com/openinput-fw/generic-mouse-boards).

## Firmware

big-sammy is meant to run on [openinput](https://github.com/openinput-fw/openinput).

## License

This hardware is licensed under the [CERN-OHL-P v2](LICENSE) license.
