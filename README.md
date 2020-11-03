# Dehydrator_PID_Nextion

This code is for a DIY PID driven dehydrator, based on a SSR (Solid state relay) to control heaters and fans, a Nextion display is used as a display/control interface.

The dehydrator code is designed for a two zones splited dehydrator, Top and Bottom, the need was to be able to use it at half capacity.

Physically it implies having 2x heaters, 2x fans (4 in my case) the Nextion control allow to start the bottom zone if needed.

To get a "synced" PWM signal for 50Hz AC 230v I use "Fast PWM to ICR1".

I've choosed to put the bottom heater/fans in parrallel to the top ones with an Y cable that connect to the SSR output that is generating the AC PWM signal, and installed a mechanical relay to on/off bottom zone.
Please be careful to choose a SSR sized to suppport the amount of current drained by heaters.

A BIG Thanks to :
- https://github.com/br3ttb and https://github.com/jackw01
- https://github.com/Seithan/
- Nick Gammon for the Timerx cheatsheets

Don't hesitate to make pull request.

Enjoy !
