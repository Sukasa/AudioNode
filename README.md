# AudioNode
ESP8266/Teensy/VS1063a-based streaming audio node with MQTT integration

This project is the motherboard for a multi-mcu audio endpoint.  It uses three CPUs; a VS1063a does the heavy lifting for the audio decoding and is operated as a slave co-processor by the ESP8266.  A Teensy 3.2 also hangs off the ESP8266, being used as a sub-processor for the touch interface (7 capacitive touch points).  The ESP controls these two processors through a shared SPI bus, with the ESP as the bus master and the Teensy/VS1063a as SPI slaves.
