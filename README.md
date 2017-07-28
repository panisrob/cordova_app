# cordova_app

Execute:

```
cordova add platform android
cordova build android
cordova run android
```

For installing:
```
cordova build --release android
keytool -genkey -v -keystore my-release-key.keystore -alias alias_name -keyalg RSA -keysize 2048 -validity 10000
jarsigner -verbose -sigalg SHA1withRSA -digestalg SHA1 -keystore my-release-key.keystore cordova_app.apk alias_name
adb install cordova_app.apk
```
