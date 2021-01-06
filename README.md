# PCU
Protocol conversion unit : A pcu which enables communication between spi and i2c interfaces.

#What is I2C?
Inter-Integrated Circuit or Two wire interface is a serial Communication Protocol which is half Duplex. Widely used for short distance, intra-board communication.
I2C connects devices like Microcontrollers, EEPROMS, A/D and D/A converters, I/O interfaces and other similar peripheral interfaces in Embedded Systems.

#TRANSMISSION OF DATA IN I2C BUS

1. IDEAL STATE: When no data is transmitted between master and slave then SDA and SCL lines are at high logic.
2. Start Condition: SDA line goes from high logic to low logic while SCL line remains  at high logic. This is called "start signal".
3. Slave Address: 7-bit address of target slave is transmitted.
4. ACK: Slave will generate a 1-bit signal to acknowledge master.
5. Data Transfer: 8-bit data is transmitted over SDA line in an order such that  MSB is   transmitted first and LSB at last.
6. ACK2: An acknowledge signal is again generated by the slave when a byte (8-bit) is received from mater.
7. Stop Condition: SDA line goes from low logic to high logic and SCL line remains high, this is called as "stop signal".




