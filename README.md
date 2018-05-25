# 使用方法
##集成步骤
1） **build.gradle**添加</br>
```
 compile 'com.github.goEcar:EcarBugly:1.1.0'
```
2）**appliction的oncreate**添加</br>
```
   BuglyUtil.init(this, BuildConfig.buglyId, false, BuildConfig.VERSION_NAME);// appid初始化
                                                     //BuildConfig.buglyId: 当前appid  false 正式环境  true 测试环境
```
3） **混淆**(不报错可不加)</br>
```
  #-dontwarn com.tencent.bugly.**
  #-keep public class com.tencent.bugly.**{*;}
```
##参考文献
[Bugly Android SDK 使用指南](https://bugly.qq.com/docs/user-guide/instruction-manual-android/?v=20170223160322)

