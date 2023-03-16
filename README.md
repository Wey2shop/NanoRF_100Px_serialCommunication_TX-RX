# NanoRF_100Px_serialCommunication_TX-RX

This project involves using Arduino to establish serial communication between a transmitter and a receiver via 2.4GHz RF communication. The purpose of this communication is to light 100 pixels connected to the receiver. The transmitter sends pixel data through Pin 6 while Pins 9 and 10 are used for cs and csn respectively.

The project uses a generic serial controller in Vixen lights. Since each pixel requires R, G, and B values (3 bytes), we need 300 channels to control all 100 pixels. Additionally, a header is used in Vixen to indicate the start of a frame, and the header in this project uses the character ">".

Each receiver board can be assigned a unique channel and address. In this project, we are using channel "124" and address "Vixen1". All data is transmitted using this channel and address combination, and the respective receivers will receive data as long as they are assigned the correct channel and address.

This project is useful for controlling large numbers of pixels and can be adapted for use in a variety of lighting applications.

**Tags:** #Arduino #RFSerialCommunication #2.4GHzRF #VixenLights #PixelControl
