# phantom-frida-17.9.1

Built from https://github.com/TheQmaks/phantom-frida

## Info

Default port has been changed to 10067 and symbol names have been changed from "frida" to "banana"

## Usage

```
adb push banana-server-17.9.1-android-arm64 /data/local/tmp/banana-server
adb shell chmod 755 /data/local/tmp/banana-server
adb shell /data/local/tmp/banana-server &
frida -H 127.0.0.1:10067 -f <package>
```
