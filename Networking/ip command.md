# Useful ip commands
Display IP addresses assigned to all interfaces (similar to ifconfig command):
```bash
ip address show
```
Show MAC address:
```bash
ip link show
```
Furthermore, you can set devices up or down (similar to ifconfig eth0 up or ifconfig eth0 down) simply by using:
```bash
ip link set DEVICE up
```
or
```bash
ip link set DEVICE down
```
More information: http://blog.cyphermox.net/2017/05/if-youre-still-using-ifconfig-youre.html.

