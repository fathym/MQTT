# MQTT for Photon, Spark Core, and Fathym
<a href="http://mqtt.org/" target=_blank>MQTT</a> publish/subscribe library for Photon, Spark Core version 0.3.5.

This version has a custom header file for MQTT.h that allows tighter integration into the <a href="http://fathym.com/" target=_blank>Fathym</a> platform, especially when building with the <a href="http://build.particle.io" target="_blank">particle.io</a> cloud build environment.

This version also contains a fix that allows MQTT packets larger than 255 bytes to be sent which allows for bigger JSON payloads to be sent to Fathym from the Photon and Spark Core.

## Source Code
This lightweight library source code are only 2 files. firmware -> MQTT.cpp, MQTT.h.

Application can use QOS0,1,2 and retain flag when send a publish message.

## Example
Some sample sketches for Spark Core and Photon included(firmware/examples/).
 - mqtttest.ino	: simple pub/sub sample. 
 - mqttqostest.ino : QoS1, QoS2 publish and callback sample.

## Arduino compatible
This library is Arduino compatible. Arduino version is <a href="https://github.com/hirotakaster/MQTT/tree/arduino">here</a>. 
