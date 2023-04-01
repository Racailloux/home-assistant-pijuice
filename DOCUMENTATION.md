# DOCUMENTATION
Here are the explainations of the various sensors added by this integration.
All data are directly readout from the PiJuice hardware and not treated/filtered. Only the status code have been adapted to texts to be human readable.

**Battery Status**
Texted value of the current status of the battery
* Normal: The battery charge is idle, the battery is charged or disconnected from power supply (discharging).
* Charging from in: The battery is charging from the USB input.
* Charging from I/O: The battery is currently charging from the GPIO bus.
* Not present: the battery is not installed and so the charging 


**Power Input status**
Texted value of the status of the power available on USB connector of the PiJuice board.
* Not present : No power is present on this port.
* Bad : Power is detected, but the voltage is pretty bad for a good charge.
* Weak : Power is detected, but the voltage is pretty weak for a good charge.
* Present : Power is detected and all is OK.


**Power input IO status**
Texted value of the status of the power available on GPIO of the PiJuice board.
* Not present : No power is present on this port.
* Bad : Power is detected, but the voltage is pretty bad for a good charge.
* Weak : Power is detected, but the voltage is pretty weak for a good charge.
* Present : Power is detected and all is OK.


**Charge**
Percentage value of the current charge of the battery connected.
```
Example : 82% => The battery needs to be charged or is discharging. Refers to the current status.
```


**Temperature**
Temperature value (°C or °F, depending of the settings of your Home Assistant installation) of the PiJuice board.
```
Example : 25°C
```


**Battery Voltage**
Voltage value of the battery connected to the PiJuice board.
Should be close to the nominal value of the battery (aka. 5 V)
```
Example : 4.088 V
```


**Battery current**
Current value of the battery connected to the PiJuice board.
Must be negative if charging, positive if discharging.
```
Example : -0.31 A
```


**IO voltage**
Voltage value available from the GPIO port.
Must be close to 5V while R.Pi is powered up and close to 0V if discharging.
```
Example : 5.134 V
```


**IO current**
Current value of the battery connected to the PiJuice board.
Must be negative if charging, positive if discharging.
```
Example : -0.2 A
```
