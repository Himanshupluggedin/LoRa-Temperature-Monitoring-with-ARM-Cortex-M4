# Temperature Monitoring using DHT11 and ARM Cortex-M4 (LPC4078)

This project interfaces a **DHT11 sensor** with an **LPC4078 ARM Cortex-M4 microcontroller** to measure and log **temperature values**. The readings are sent over **UART0** to a serial terminal.

---

## Hardware

- LPC4078 ARM Cortex-M4
- DHT11 Temperature Sensor
- FT232H Module
- 3.3V Power Supply

**Connections**
| LPC4078 Pin | Function |
|--------------|-----------|
| P4.0 | DHT11 Data |
| P0.2 | UART0 TX |
| P0.3 | UART0 RX |

---

## Software

- Keil µVision 
- Flash Magic 
- Hyper Terminal 

---

## Working

1. LPC4078 sends a start signal to DHT11.  
2. The sensor responds with digital temperature data.  
3. The MCU converts the value to ASCII and transmits via UART0.  
4. Output is displayed on the serial terminal every few seconds.
