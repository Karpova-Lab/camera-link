# Hardware
## Camera Stuff
- [Chameleon3 USB3](https://www.flir.com/products/chameleon3-usb3/?model=CM3-U3-31S4C-CS)
    - [Technical Rererence](datasheets/CM3-U3-Technical-Reference.pdf)
- [GPIO Connector](https://www.flir.com/products/jst-gpio-connector-for-chameleon-3/)
- [Lens](https://www.flir.com/products/computar-a4z2812cs/)

## Camera connection pinout
| GPIO pin | GPIO Color | GPIO Function | RJ45 Pin | pyControl Function | Purpose                                                  |
|----------|------------|---------------|----------|--------------------|----------------------------------------------------------|
| 4        | Green      | GPIO3/Line3   | 1        | DIO_A              | pyControl sends square wave to camera to grab each frame |
| 9        | Yellow     | OPTO_IN/Line0 | 4        | DIO_B              | pyControl sends random sync pulse                        |
| 6        | Black      | GND           | 2        | Ground             | Ground                                                   |
| 7        | Brown      | OPTO_GND      | 2        | Ground             | Ground                                                   |

## PCB bill of materials
| Qty | Reference | Description       | Value/MPN                                                                                                                                      | 
|-----|-----------|-------------------|------------------------------------------------------------------------------------------------------------------------------------------------|
| 24  | D1-D24    | 850nm 140˚ LED    | [15412085BA400](https://www.digikey.com/en/products/detail/15412085BA400/732-15412085BA400CT-ND/12385059?itemSeq=350631554)                    | 
| 2   | H1, H2    | Threaded Standoff | [24882](https://www.digikey.com/en/products/detail/keystone-electronics/24882/9921822?s=N4IgTCBcDaIMwDYC0YAsAOdYkEYkDkAREAXQF8g)               | 
| 1   | J1        | RJ45 Jack         | [0855025008](https://www.digikey.com/en/products/detail/molex/0855025008/2404887?s=N4IgTCBcDaIOoFkDMBWALAdgMIBUC0AcgCIgC6AvkA)                 | 
| 1   | R1        | 1206 Resistor     | [10Ω](https://www.digikey.com/en/products/detail/bourns-inc/CMP1206AFX-10R0ELF/12333667?s=N4IgTCBcDaIMIFkAKBGMAGAbAQQGIA0BaFdAJXQFEAZXEAXQF8g) | 

# Software
- [Bias](http://stuff.iorodeo.com/notes/bias/)
- [pyControl synchronization](https://pycontrol.readthedocs.io/en/latest/user-guide/synchronisation/)