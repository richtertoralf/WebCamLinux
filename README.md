# WebCamLinux
WebCams anschließen

```
sudo apt update 
sudo apt install v4l-utils
```

USB Geräte anzeigen:  
`v4l2-ctl --list-devices`  

verfügbare Steuerelemente anzeigen:  
`v4l2-ctl -d /dev/video3 --list-ctrls`  

aktuellen Wert anzeigen, z.B.:  
`v4l2-ctl --get-ctrl=white_balance_temperature`  

Werte einstellen, z.B.:  
```
v4l2-ctl --set-ctrl=gain=00
v4l2-ctl --set-ctrl=exposure_auto=1
v4l2-ctl --set-ctrl=exposure_absolute=10
```
