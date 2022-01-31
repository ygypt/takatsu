#### create filesystem
+ format to fat32
+ use raspberry pi image tool (or etcher but its fucky) to flash sd card with **raspbian lite** iso

#### configure
+ copy contents of `boot` to the `/boot` directory in sd card [an empty `ssh` file and a `wpa_supplicant.conf` template]
+ edit `wpa_supplicant.conf` to include the correct SSID and PASS
+ edit `config.txt` in the `/boot` directory: uncomment `#config_hdmi_boost=4`
+ copy everything else in this repo into `/home/pi/`

#### initial setup
+ insert sd card, power on pi
+ login to user: `pi` pass: `raspberry`
+ `passwd`
+ `sudo apt install xorg feh`
+ `startx`

#### ssh
+ you can now `scp` a new `takatsu.png` into `/home/pi/` and feh will automatically update the picture within 60 seconds
