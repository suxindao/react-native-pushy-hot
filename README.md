# react-native-pushy-hot

RN的测试用例，附带了使用RN.cn的pushy热更新服务

## React Native 中文网
    http://reactnative.cn/docs/0.39/getting-started.html
    
## Pushy 热更新
    http://update.reactnative.cn/home
    
1. 编译APK
```
cd android
./gradlew assembleRelease
```

2. 上传APK
```
cd ..
pushy uploadApk android/app/build/outputs/apk/app-release.apk
```

3. 上传更新
```
    suxindao@bogon:~/work/XNJH/app/Hello$ pushy bundle --platform android
    Bundling with React Native version:  0.39.1
    [12/13/2016, 4:29:37 PM] <START> Initializing Packager
    [12/13/2016, 4:29:37 PM] <START> Building in-memory fs for JavaScript
    [12/13/2016, 4:29:38 PM] <END>   Building in-memory fs for JavaScript (138ms)
    [12/13/2016, 4:29:38 PM] <START> Building Haste Map
    [12/13/2016, 4:29:38 PM] <END>   Building Haste Map (816ms)
    [12/13/2016, 4:29:38 PM] <END>   Initializing Packager (1063ms)
    [12/13/2016, 4:29:38 PM] <START> Transforming files
    [12/13/2016, 4:29:39 PM] <END>   Transforming files (411ms)
    bundle: start
    bundle: finish
    bundle: Writing bundle output to: /Users/suxindao/work/XNJH/app/Hello/build/intermedia/android/index.bundlejs
    bundle: Copying 5 asset files
    bundle: Done writing bundle output
    bundle: Done copying assets
    Packing
    Bundled saved to: build/output/android.1481617776065.ppk
    Would you like to publish it?(Y/N) Y
      Uploading [================================================================================================================================================================================================================================================] 100% 0.0s
    Enter version name: 1.0.2
    Enter description: 热更新
    Enter meta info: update:2
    Version published: 9596
    Would you like to bind packages to this version?(Y/N) Y
    4446) 1.0(normal) - 9584 FsvkqW_w 1.0.1-rc
    
    Total 1 packages.
    Enter packageId: 4446
    Ok.
```


    