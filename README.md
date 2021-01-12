# lib-zxing-replugin
 

查看 [android-zxingLibrary官方使用说明](https://github.com/yipianfengye/android-zxingLibrary)

## 说明

最新项目使用了Replugin,android-zxingLibrary闪退，是因为android-zxingLibrary提供的Activity没有继承Replugin的Activity的问题，分享出来供使用插件化的小伙伴继续使用android-zxingLibrary

宿主包使用官方的集成
插件包使用此集成

> 添加依赖

`root build.gradle `
```
allprojects {
    repositories {
        ...
        maven {
            url 'https://jitpack.io'
        }
    }
}
```
`module build.gradle `
```
implementation 'com.github.fonuhuolian:lib-zxing-replugin:0.0.1'
```

## Thanks
感谢yipianfengye大神 [android-zxingLibrary](https://github.com/yipianfengye/android-zxingLibrary)
