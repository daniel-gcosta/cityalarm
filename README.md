# cityalarm
Implementation of the CityAlarm Emergency Alerting system (and an extension for visual sensing), which were developed in 2019/2020 by Prof. Daniel G. Costa.

The scientific papers associated to this repository are: A Distributed Multi-Tier Emergency Alerting System Exploiting Sensors-Based Event Detection to Support Smart City Applications (https://doi.org/10.3390/s20010170), and On the Use of Cameras for the Detection of Critical Events in Sensors-Based Emergency Alerting Systems (https://doi.org/10.3390/jsan9040046).

The CityAlarm implementation is divided in three elements:

Events Dectection Unit (EDU), Emergencies Processing Unit (EPU), and Emergency Alarms Client (EAC).

All codes are written in Python3, using some additional libraries.

*******************************************************************

The EDU is implemented around the GrovePi+ hardware framework.

The GrovePi+ has to be installed and enabled, as specified by the manufacturer. The following link describes all the required steps to allow the use of GrovePi+ in the Raspberry Pi: https://www.dexterindustries.com/GrovePi/get-started-with-the-grovepi/

Before using the EDU, one additional library has also to be installed through the following command:

pip3 install numpy

As a second remark about the EDU and the GrovePi+, the GPS module operates through the serial port of Raspberry and thus the Bluetooth module needs to be deactivated in some versions

*******************************************************************

For the EPU, the haversine lib has to be installed:

pip3 install haversine

For the EPU and the EAC, the paho-mqtt library has also to be installed, using the follwing command:

pip3 install paho-mqtt

*******************************************************************

If the EACMap app is used, the folium library has to be installed through the following command:

pip3 install folium
