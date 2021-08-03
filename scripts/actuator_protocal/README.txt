V010 connect actuator communication using uart2

follow next step

1. active dtoverlay
	edit /boot/firmware/usercfg.txt
	add line "dtoverlay=uart2"
	reboot
2. install minicom
	apt-get install minicom

3. setting minicom
	run "minicom -s"
	select Serial port setup
	A - Serial device = /dev/serial1
	E - Bps = 1500000 8N1

4. confirm communication
	type "act [num]"
	you can see return value and success


if not working..

	fix /boot/firmware/config.txt
	delete "enable_uart=1
