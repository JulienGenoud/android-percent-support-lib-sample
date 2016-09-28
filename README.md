Android Percent Support Lib Sample :triangular_ruler::triangular_ruler::triangular_ruler:
===================================
[![Android Arsenal](https://img.shields.io/badge/Android%20Arsenal-android--percent--support--lib--sample-green.svg?style=flat)](https://android-arsenal.com/details/3/2054)

I made a sample of the new percent support library.<br>
You can check official docs reference [here](https://developer.android.com/reference/android/support/percent/package-summary.html) 
and [here](https://developer.android.com/tools/support-library/features.html#percent).<br>
This library provide percentage based layouts,
horizontal and vertical at the same time.

## simple result
![PercentRelativeLayout](https://cloud.githubusercontent.com/assets/1808854/8392086/dd20ee1e-1cdd-11e5-852e-795a0d00cc89.png)
## complex result
![PercentRelativeLayout Complex](https://cloud.githubusercontent.com/assets/1808854/8398283/22bd374c-1de8-11e5-9e74-f19ea46b8086.png)




### How to use :
just add percent support library to your project
```xml
dependencies {
    compile 'com.android.support:percent:22.2.0'
}
```

###Supported Layouts :

####PercentRelativeLayout
```xml
<android.support.percent.PercentRelativeLayout
    xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    android:layout_width="match_parent"
    android:layout_height="match_parent">
    
    <View
        android:id="@+id/top_left"
        android:layout_width="0dp"
        android:layout_height="0dp"
        android:layout_alignParentTop="true"
        android:background="#ff44aacc"
        app:layout_heightPercent="20%"
        app:layout_widthPercent="70%" />

    <View
        android:id="@+id/top_right"
        android:layout_width="0dp"
        android:layout_height="0dp"
        android:layout_alignParentTop="true"
        android:layout_toRightOf="@+id/top_left"
        android:background="#ffe40000"
        app:layout_heightPercent="20%"
        app:layout_widthPercent="30%" />


    <View
        android:id="@+id/bottom"
        android:layout_width="match_parent"
        android:layout_height="0dp"
        android:layout_below="@+id/top_left"
        android:background="#ff00ff22"
        app:layout_heightPercent="80%" />
</android.support.percent.PercentRelativeLayout>
```

####PercentLinearLayout
```xml
<com.juliengenoud.percentsamples.PercentLinearLayout
    xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:orientation="vertical">
     <View
        android:layout_width="0dp"
        android:layout_height="0dp"
        android:background="#ff44aacc"
        app:layout_heightPercent="10%"
        app:layout_widthPercent="60%"/>

    <View
        android:layout_width="0dp"
        android:layout_height="0dp"
        android:background="#ff4400cc"
        app:layout_heightPercent="10%"
        app:layout_widthPercent="70%"/>
</com.juliengenoud.percentsamples.PercentLinearLayout>
```

####PercentFrameLayout
```xml
<android.support.percent.PercentFrameLayout
    xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    android:layout_width="match_parent"
    android:layout_height="match_parent">
        <!-- ... XML CODE -->
</android.support.percent.PercentFrameLayout>
```



###Stylable :

- heightPercent
- widthPercent
- marginBottomPercent
- marginEndPercent
- marginLeftPercent
- marginPercent
- marginRightPercent 
- marginStartPercent
- marginTopPercent

Pre-requisites
--------------

- Android SDK v22
- Android Build Tools v22.0.1
- Android Percent Support Repository v22.2.0
- Android Support v4 Repository v22.2.0

according to the the manifest minsdk is v7 (android 2.1) 

####License Mit
