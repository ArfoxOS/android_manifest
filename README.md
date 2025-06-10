![banner](https://raw.githubusercontent.com/ArfoxOS/android_manifest/refs/heads/15/res/banner.png)
## Getting started

To get started with Android/ArfoxOS, you'll need to get familiar with [Source Control Tools](https://source.android.com/setup/develop).

## Sync sources

To initialize your local repository using the ArfoxOS trees, use a command like this:
```
repo init -u https://github.com/ArfoxOS/android_manifest -b 15 --git-lfs
```
Then to sync up:
```
repo sync
```

## Building

To start building, you should set first the target
```
lunch arfox_{devicename}-bp1a-{variant}
```
- devicename is the device name (lemonadep, Pong, munch...)
- variant is the type of build (eng, user, userdebug)

Then we can start the build
```
make berries -j$(nproc)
```