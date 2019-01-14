## Connect to matooma
1. Turn on the modem.
2. Run `pon`
  * Eventually check logs `tail -f /var/log/messages`
3. Change bridge
  List connections : `ip route list` en search for ppp
  Remove default wifi `sudo ip route del default`
  Set new default to ppp `sudo ip route add default via xxx.xxx.xxx.xxx`
