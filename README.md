## Connecting and testing the module nRF24L01+
##### To work with the module, you must first enable SPI
To enable SPI, use `raspi-config` or uncomment the line `dtparam=spi=on` in `/boot/config.txt`. Reboot afterwards.
Upon successful loading of the SPI driver, you will see the device `/dev/spidev0.0`.
#### Compiling and building :
```sh
$ g++ -Wall scanner.cpp -o scanner -lrf24 
```
#### Wiring diagram nRF24L01+ to Raspberry Pi :
![scheme](https://github.com/wirekraken/Raspberry-Pi-NRF24/blob/master/scheme/scheme.png)

