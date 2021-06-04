## WALLPANEL

1. **[Fire-OS](#fire-os)**
2. **[Disable lockscreen](#disable-lockscreen)**

<br/>

## Fire-OS

```
1) Install Settings Database Editor.apk

2) Settings > Device Options > tap on the Serial Number until you unlock Developer Options

3) adb shell
   pm grant by4a.setedit22 android.permission.WRITE_SECURE_SETTINGS
```

## Disable lockscreen

```
secure 	lockscreen_disabled 	1
global 	device_provisioned 	0
```
