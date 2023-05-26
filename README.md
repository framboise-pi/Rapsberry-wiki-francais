SYNTAX GITHUB
https://docs.github.com/fr/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax

# Rapsberry-wiki-francais
Wiki pour annoter les choses Raspberry-utiles que j'ai trouvé sur le passage

![Pi logo](https://www.raspberrypi.com/app/uploads/2022/02/COLOUR-Raspberry-Pi-Symbol-Registered.png)

### QWERTY -> AZERTY
setxkbmap fr

### LISTER PERIPHERIQUES USB
`lsusb`

### TERMINAL | passer en ROOT
`sudo -s`

### CAMERA | éteindre LED rouge
éditer le fichier config.txt
<br>`sudo nano /boot/config.txt`
<br>`disable_camera_led=1`

### PI-HOLE
blacklists
https://firebog.net/

### PHP 8.1 INSTALLATION
<br>un mélange entre ces deux pages pourq ue ça marche:
<br>https://pimylifeup.com/raspberry-pi-latest-php/
<br>https://www.tal.org/tutorials/setup-php-7-or-8-apache-raspberry-pi

### PI ZERO WIFI
Sur la partition /boot de la carte µSD,
créer un fichier "wpa_supplicant.conf"

<br>`ctrl_interface=DIR=/var/run/wpa_supplicant GROUP=netdev`
<br>`update_config=1`
<br>`country=US`
<br>
<br>`network={`
<br>`     ssid="Your network name/SSID"`
<br>`     psk="Your WPA/WPA2 security key"`
<br>`     key_mgmt=WPA-PSK`
<br>`}`
