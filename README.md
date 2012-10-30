EasyTracker
===========

EasyTracker with Fragments support for Google Analytics EasyTracker library.

Original library can be found in the downloads section of the analytics-api-samples project:

https://code.google.com/p/analytics-api-samples/  
https://code.google.com/p/analytics-api-samples/downloads/

What is different
-------------
- Supports Fragments out of the box
- Has the analytics library included
- Has a better implementatino of the EasyTracker as a singleton


Setup
-------------
* Clone the repo
* Import as existing project into your workspace
* Reference the EasyTracker library project in your own project

NOTE: you don't need to add any additional libraries. This repository is self contained.

You may want to add a config file to your _/res/values/_ folder

```xml
<?xml version="1.0" encoding="utf-8"?>
<resources>

    <string name="ga_api_key">UA-XXXXXXXX-X</string>

    <bool name="ga_debug">true</bool>
    <bool name="ga_auto_activity_tracking">true</bool>
    <bool name="ga_anonymizeIp">true</bool>

    <item name="ga_dispatchPeriod" format="integer" type="integer">120</item>

</resources>
```


Don't forget to add networking permissions to your **AndroidManifest.xml**

```xml
<uses-permission android:name="android.permission.INTERNET" />
<uses-permission android:name="android.permission.ACCESS_NETWORK_STATE" />
```