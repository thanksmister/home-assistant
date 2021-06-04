You can't take my APK file that belongs to my open source project and use it in your own project.  You must refer back to my project because I own that APK and the code and you have to credit my project.   Please remove the WallPanel apk from your project. 

## WALLPANEL

1. **[Fire-OS](#fire-os)**
2. **[Disable lockscreen](#disable-lockscreen)**

<br/>

https://forum.xda-developers.com/t/disable-swipe-up-lockscreen.4032599/


## Fire-OS
```
Alimentation: Désactiver toutes les options d'économie d'énergie
Affichage: Désactiver luminosité adaptive
Mise en veille de l'écran: 5 minutes
Orientation: Conserver l'orientation portrait
Services de localisations: Désactiver toutes les options
Administrateurs de l'appareil: Désactiver Mode Show
```


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
