## Master Controller


####Master Controller as Failsafe Controller

Master controller can serve as a failsafe controller while developing on Slave Controller. In this mode ensure that off-board control is given on RC transmitter. By default **Channel 7** is used for that purpose. On Futaba TX supplied with the setup it is **Switch G**.
While switching the master is put into offboard mode and accepts unmixed motor commands from Slave Controller. The communication protocol used between master and slave is [UAVCAN](http://uavcan.org/).


####Master Controller as Sole Flight controller
It is also possible to use it as the main controller that interacts withonboard computer. To use it as the sole controller ensure that Master USB port on Flight Board is connected to onboard computer.

{% hint style='info' %}
Try not to modify PX4 Firmware on Master Controller for your and drones safety, if you need to develop on Autopilot end use the first mode of operation.
{% endhint %}





