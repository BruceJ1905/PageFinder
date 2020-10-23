# PageFinder

Welcome to the PageFinder wiki!

# What's it ?
It's a helper tool for Android developers.  
It can monitor current launched activity or fragment and logcat correspond Class Name.  
So that we can quick locate to the source code.

# How to use ?  
##   1. project build.gradle 
    repositories {
		google()
		jcenter()
            maven { url 'https://jitpack.io' }
    }

##  2. app build.gradle 

    implementation 'com.github.BruceJ1905:PageFinder:1.0.4'

##  3. Application onCreate
    PageFinder.init(this, BuildConfig.DEBUG);

=============================

Then filter log tag "PageFinder" and enjoy it !

adb logcat -s 'PageFinder'

You can get every launched activity or fragment Class name in debug mode.  

It won't work in release mode. So don't worry about impacting your App performance.

=============================

# Contact me 

pls contact me if you have any question.

Email:  brjiang@coupang.com


PageFinder   VS     [CurrentActivity](https://github.com/BruceJ1905/CurrentActivity)

|  PageFinder   | [CurrentActivity](https://github.com/BruceJ1905/CurrentActivity)  |
|  ----  | ----  |
| 嵌入项目源码  | 无需嵌入源码 |
| 检测activity， fragment  | 检测activity，dialog， view |
| maven库  |   apk   |
| lifecycle callback   |    辅助服务AccessibilityService  | 
