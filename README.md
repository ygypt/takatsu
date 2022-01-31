+ use raspberry pi image tool (or etcher but its fucky) to flash sd card with **raspbian lite** iso
+ copy contents of `boot` to the `/boot` directory in sd card [an empty `ssh` file and a `wpa_supplicant.conf` template]
+ edit `wpa_supplicant.conf` to include the correct SSID and PASS
+ copy everything else in this repo into `/home/pi/`
+ insert sd card, power on pi, ssh into user: `pi` pass: `raspberry`
+ `passwd`
+ `sudo apt install xorg feh`
+ `startx`

+ you can now `scp` a new `takatsu.png` into `/home/pi/` and feh will automatically update the picture within 60 seconds
