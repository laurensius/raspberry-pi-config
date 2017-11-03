# Raspberry Pi Configuration
<h1>Setup Auto Connect Wifi</h1>
<ul>
<li>Buka terminal</li>
<li>Masukkan kode di bawah ini 
<br>
sudo nano /etc/network/interfaces
</li>
<li>Masukkan kode di bawah ini 
<br>
auto lo
 
iface lo inet loopback
iface eth0 inet dhcp
 
allow-hotplug wlan0
auto wlan0
 
 
iface wlan0 inet dhcp
        wpa-ssid "ssid"
        wpa-psk "password"
</li>
  
</ul>
