# ResEnv-showcase-video-looper

1. connect the Raspberry Pi zero with the display with FPC HDMI cable and a Micro USB to Micro USB cable;
2. Use the img Raspberry Pi OS Lite (Legacy): https://www.raspberrypi.com/software/operating-systems/#raspberry-pi-os-legacy for raspberry pi (the Lite version, the one with graphic interface will causse the RPi over ehat and crash)
3. Set up the Pi WiFi connection by command $ raspi-config -> Network -> SSID -> password;
4. Set up resolution by command $ raspi-config -> display configuration -> resolution;
5. checking the hostname of the Pi: ''' hostname -I '''
6. ssh to Pi: ssh pi@IP address got from the last step;
7. install omxplayer: $ sudo apt-get install omxplayer;
8. copy video files from host machine: https://unix.stackexchange.com/questions/106480/how-to-copy-files-from-one-machine-to-another-using-ssh
9. Command line for looping video: omxplayer -o local --loop /path/to/video/file
10. set the video looping begin at the start up: https://www.dexterindustries.com/howto/run-a-program-on-your-raspberry-pi-at-startup/, I used the rc.local approach.
