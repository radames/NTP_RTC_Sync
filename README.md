# Sync RTC clock with NTP 

## Libs

You must have the libs:

* [Adafruit RTCLib](https://github.com/adafruit/RTClib)
* [Arduino NTP Client](https://github.com/arduino-libraries/NTPClient)

You can install from Arduino/ Manage Libraries menu

## Wifi

Copy `WifiPass.h.config` to `WifiPass.h` and change the `ssid` and `password` to your wifi network information.

## Parameters
Change the `NTP_SERVER` to a suitable server.

```C
#define NTP_SERVER "0.us.pool.ntp.org"
```

Change the GMT time zone `GMT_TIME_ZONE` you can add a signed number 

```C
#define GMT_TIME_ZONE -7
```

You can force the time sync after the first time changing the `FORCE_RTC_UPDATE` to a random number between 0-255
```C
#define FORCE_RTC_UPDATE 2
```
