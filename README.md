## Clash for Android

A Graphical user interface of [clash](https://github.com/Dreamacro/clash) for Android

<a href="https://play.google.com/store/apps/details?id=com.github.kr328.clash"><img width="200px" alt="Get it on Google Play" src="https://play.google.com/intl/en_us/badges/static/images/badges/en_badge_web_generic.png"/></a> or [Releases](https://github.com/Kr328/ClashForAndroid/releases)

### Feature

Fully feature of [clash](https://github.com/Dreamacro/clash) ~~(Exclude `external-controller`~~

Support [ShadowsocksR](https://github.com/mzz2017/shadowsocksR)


### Requirement

* Android 7.0+
* `armeabi-v7a` , `arm64-v8a`, `x86` or `x86_64` Architecture

### License

See also [LICENSE](./LICENSE) and [NOTICE](./NOTICE)



###  Privacy Policy

See also [PRIVACY_POLICY.md](./PRIVACY_POLICY.md)



### Build

1. Update submodules

   ```bash
   git submodule update --init --recursive
   ```

2. Install `JDK 1.8`, `Android SDK` ,`Android NDK` and `Golang`

3. Create `local.properties` in project root with 

   ```properties
   sdk.dir=/path/to/android-sdk
   ndk.dir=/path/to/android-ndk
   appcenter.key=<AppCenter Key>    # Optional, from "appcenter.ms"
   ```

4. Create `keystore.properties` in project root with

   ```properties
   storeFile=/path/to/keystore/file
   storePassword=<key store password>
   keyAlias=<key alias>
   keyPassword=<key password>
   ``` 

5. Build

   ```bash
   ./gradlew app:assembleRelease
   ```

6. Pick `app-release-<arch>.apk` in `app/build/outputs/apks`
