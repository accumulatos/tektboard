# A Mongoose OS library with pin constants for the Tekt Board
A couple of things to note:
- Due to Mongoose OS limitations, pin A0 and A1 (to which the Grove Analog pins
are connected) are not supported as they use ADC2 rather than ADC1 inside the
ESP32. To overcome this, a small modification was made to the board to join
pin AN0 to AN2, as AN2 is connected to ADC1. To make this adjustment easier,
AN1 was cut to disconnect it in case it was shorted to AN0/2.
