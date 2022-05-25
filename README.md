[![](https://jitpack.io/v/team-telnyx/telnyx-meet-android-sdk.svg)](https://jitpack.io/#team-telnyx/telnyx-meet-android-sdk)

# telnyx-video-android

## Adding Telnyx to your Android client application

1. Add Jitpack.io as a repository within your root level build file:
```groovy
allprojects {
		repositories {
			...
			maven { url 'https://jitpack.io' }
		}
	}
```
2. Add the dependency within the app level build file:
```groovy
dependencies {
	implementation ('com.github.team-telnyx:telnyx-meet-android-sdk:0.2.5@aar'){transitive=true}
	}
```

Note that '0.2.3' should be replaced with the newest version represented by the Jitpack badge

Tag should be replaced with the release version.
<br>
<br>
Then, import the TelnyxVideo SDK into your application code at the top of the class:

```kotlin
import com.telnyx.video.sdk.*
```

The ‘*’ symbol will import the whole SDK which will then be available for use within that class.
<br>
<br>
NOTE: Remember to add and handle INTERNET, RECORD_AUDIO and ACCESS_NETWORK_STATE permissions in order to properly use the SDK

```groovy
    <uses-permission android:name="android.permission.INTERNET"/>
    <uses-permission android:name="android.permission.CAMERA"/>
    <uses-permission android:name="android.permission.RECORD_AUDIO"/>
    <uses-permission android:name="android.permission.MODIFY_AUDIO_SETTINGS"/>
```
<br>
