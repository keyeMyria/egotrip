GPS Tracking they way YOU decide
================================

Egotrip is an android application for tracking your gps location and instantly upload it to a webserver of your choice. You can then display your current location or a whole trail the way you like it


Features
========


 *  Records your current position in configurable intervals
 *  Instant upload (can be disabled to save bandwidth)
 *  attach text and images to your locations
 *  View and edit current trip on map
 *  Profile View

Please visit http://www.myegotrip.net/ for more details and screenshots

APK Download
============

https://play.google.com/store/apps/details?id=net.myegotrip.egotrip


Build Instructions
==================

 * google maps api key in res/layout/map.xml (TODO - app was built with maps api v1 but apparently you can no longer get api keys?)
 

Developer Info & Tools
======================

Editing the local SQLite Database
---------------------------------

	adb shell
	cd /data/data/net.myegotrip.egotrip/databases
	sqlite3 egotrip

Manually Set GPS Location in the Emulator
-----------------------------------------

	telnet localhost 5554
	Trying ::1...
	Connection failed: Connection refused
	Trying 127.0.0.1...
	Connected to localhost.
	Escape character is '^]'.
	Android Console: type 'help' for a list of commands
	OK
	geo fix 8.502061 47.421909

