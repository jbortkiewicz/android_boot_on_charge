# Android Boot on Charge

This is short intruction to enable automatic booting when plug in charger.

**ROOT required**

To enable automatic booting edit `/init.rc` and replace:
```
on charger
    class_start charger
```
with:
```
on charger
    setprop sys.powerctl reboot
```
