phue-daynight
=============

Simple Python script to turn Philips Hue Lights on/off according to sunset/sunrise.
Its basicly a wrapper script around 'ephem' and 'phue' functions. 
- Ephem to calculate the sunset/sunrise times from gps coordinates.
- Phue to interface with the Philips Hue lighting system.

Its designed to run scheduled on a designated time interval.
I run the script each 15minutes with a cronjob on a QNAP TS-212.
There are other ways to achief the same results offcorse, but this works best in my setup

Example cron usage:
*/15 * * * * /opt/bin/python2.7 /share/MD0_DATA/phue-daynight/daynight.py >/dev/null 2>&1


Python library dependencies:
datetime, ephem and phue

These can be installed with pip:
$ pip install ephem
$ pip install datetime
$ pip install phue

