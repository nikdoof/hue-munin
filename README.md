Philips Hue Munin Plugin
========================

A Munin plugin to take advantage of sensor data provided by Philips Hue motion sensors. The sensors provide Temperature (in degrees celcius) and Light Level (in lux).

Requirements
------------

* Requests
* [python-munin](https://github.com/samuel/python-munin)

Modes
-----

* ```hue_temperature``` returns graphs showing all temperature sensors.
* ```hue_lightlevel``` returns the light level.
* ```hue_all``` shows a combination graph of all values.

Munin Configuration
-------------------

These values will be set in your ```plugin-conf.d/munin-node``` file.

* ```hub_address``` - IP address of the Philips Hue hub
* ```api_key``` - API Key/User ID to access the Hue API. 

Example Config
--------------

    [hue_*]
    env.hub_address 10.1.1.2
    env.api_key test1234