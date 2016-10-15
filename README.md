## <p>Sample App:</p>
<a href="https://play.google.com/store/apps/developer?id=Matteo+Battilana"><img alt="Get it on Google Play" src="https://play.google.com/intl/en_us/badges/images/apps/en-play-badge-border.png" width="300" /></a>


Or you can download <a href="https://github.com/MatteoBattilana/WeatherView/raw/master/app/app-release.apk">WeaterView Library Demo apk</a> to check out what can be done with it.

#WeatherView

WeatherView is an Android Library that helps you make a cool weather animation for your app.

<img src="https://github.com/MatteoBattilana/WeatherView/blob/master/Screenshot/home.gif" width="500">

<img src="https://github.com/MatteoBattilana/WeatherView/blob/master/Screenshot/device-2016-10-15-152953.png" width="250">
<img src="https://github.com/MatteoBattilana/WeatherView/blob/master/Screenshot/device-2016-10-15-153044.png" width="250">
<img src="https://github.com/MatteoBattilana/WeatherView/blob/master/Screenshot/device-2016-10-15-153100.png" width="250">




##Setup
###Android Studio / grandle
Add the following dependency to the **build.gradle** of your project:

``` 
repositories {
	maven { url = 'https://jitpack.io' }
}

dependencies {
	compile 'com.github.MatteoBattilana:WeatherView:1.0.5'
}
```

###Basic usage
Open an Activity:
``` Java
        WeatherView mWeatherView = (WeatherView) findViewById(R.id.weather);
        //Optional
        mWeatherView.setWeather(WeatherView.weatherStatus.RAIN);
        mWeatherView.startAnimation();
```

Include into activity_main.xml
``` Xml
<xyz.matteobattilana.library.WeatherView
        xmlns:app="http://schemas.android.com/apk/res-auto"
        android:id="@+id/weater"
        android:layout_width="match_parent"
        android:layout_height="1dp"
        app:fadeOutTime="1000"
        app:liveTime="3000"
        app:startingWeather="RAIN" />
```
