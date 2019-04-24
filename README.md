![Header](https://github.com/regenhans/open_swim_ble_risc-V/blob/master/img/github.png)

A lap counter device  for swiming training

This repo is based on the "heart_rate_monitor" demo provided by NXP

## Working demo capabilities

The current version of this software allows the Vega Board to become a data streamer of one type of event: "laps".
The laps are send through BLE to the connected devices (tested 4 simultaniously).

Unfurtunatelly the working demo laks the full integration with the ultrasonic sensor due to PWM issues that I were unable to solve. However I'm simulating the event using the built in SW and you can check my working demo of the sensor working on arduino [here](https://github.com/regenhans/lap_notify_service) as well as the technichal diagrams for the implementation on the vega board. 

The streaming of data as well as the input source are  working properly and my mobile applications can detect the changes inmediatly.

## Constraints of the ultrasonic sensor.

The sensor can work over the watter and just passing the surface of the watter, it's safe to say that it behaves more reliably over due to sound moving at different speed under watter and it's very dificul to recalibrate on site. So right now it can only detect over the watter motion. It could be interesting to try a more powerfull sonar next time :b .

