# experiment_shorebird

Basic app to try out Shorebird, contains a build and a patch.

## APK

Created the APK from the release's aab via 
```
java -jar bundletool-all-1.17.0.jar build-apks --bundle=my_app.aab --output=my_app.apks \
--ks=keystore.jks \
--ks-pass=<keystorepass> \
--ks-key-alias=<keyalias> \
--key-pass=<keypass>
```

Download via:

![QR Code for APK](download_qr.jpg)

First launch you should see an incorrect text. Second launch it should update to the correct patched version. (After swiping away from recents)

## Local development

Steps:
 - install FVM
 - fvm use
 - install shorebird
 - define aliases for flutter
```
alias f="fvm flutter"
alias flutter="fvm flutter"
```
 - shorebird login
