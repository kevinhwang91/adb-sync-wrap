## ADB Sync Wrap

ADB Sync Wrap is a tool to enhance [adb-sync](https://github.com/google/adb-sync).

---

## Setup

require: [adb-sync](https://github.com/google/adb-sync)
option: [GSConnect](https://github.com/andyholmes/gnome-shell-extension-gsconnect)

---

## Usage
To get a full help, type:

```
adb-sync-wrap --help
```

To Sync qqmusic and neteasecloud from your PC to your device, type one of:

```
adb-sync-wrap -o ~/Music/qq/,~/Music/netease/ /sdcard/qqmusic/song/,/sdcard/netease/cloudmusic/Music/
```

To Sync qqmusic and neteasecloud from your device to your PC, deleting files you removed from your device, type one of:

```
adb-sync-wrap -d -i ~/Music/qq/,~/Music/netease/ /sdcard/qqmusic/song/,/sdcard/netease/cloudmusic/Music/
```

If using GSConnect to connect adb by wireless, to sync music from your device to your pc, trigger by your PC terminal, type one of :

```
adb-sync-wrap -k name_of_device_in_gsconnect_app -i ~/Music/qq/ /sdcard/qqmusic/song/
```

If using GSConnect to connect adb by wireless, execute the shell to sync music from your device to your pc, trigger by your device inside GSConnect app, build a shell like this:

```
adb-sync-wrap -g -k name_of_device_in_gsconnect_app -i ~/Music/qq/ /sdcard/qqmusic/song/
```

