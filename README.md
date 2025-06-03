# ITECH-N6962
CAPL code to control ITECH 6900 series Power Supply

First make the Power supply to REM (Remote Enable Mode) Mode. On REM Mode only, the Power supply will accept the command.![image](https://github.com/user-attachments/assets/01ad6277-f8ac-431c-8134-8ba7f6201f94)

When we connect the power supply using USB to the PC, REM Mode will already enable and we can see the REM Mode enable icon on Power supply.

When we connect the power supply using RS232 to the PC, REM Mode will enable by sending the command SYST:REM


"Remote_Control_ITECH_N6962.can" is the updated code in which we reduce the size of the code and also implemented Over Voltage Protection (OVP) using CAPL. Also we limit voltage:  if the Input Voltage > 18.5, Output Voltage is maximum = 18.5.
