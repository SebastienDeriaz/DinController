# DinController

Din-format controller board for simple automation and IoT


## 15.04.2023


### Mechanical

- DIN format
- 4-layer stack :
  1) Power-supply and inputs / outputs
  2) CPU
  3) Communication (4G, LoRa, etc...)
  4) UI (screen, buttons, leds, etc...)
  
### User interface

- User interface connector (USB C + FTDI most likely) to configure and retrieve data from the controller
- Status screen with potential pages support
- User menus at a minimum (USB interface is preferred)

### Power

- Two connectors : battery and input power
  1) 0-24 V power supply that can also accomodate solar power input
  2) External battery connector (Lithium and/or lead acid)
- Potential onboard battery
- IOs have dedicated extzenal power input
- A regulated power output could be implemented (to power the IOs from the battery for example)
  - Could be switched / configured between (5), 12 and/or 24V

### Software

- Command interpreter for both onboard UART and remote configuration (the same commands can be received by USB or wirelessly to configure the module)
