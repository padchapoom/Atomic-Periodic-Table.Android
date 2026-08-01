###413582853428#1749900456329#  'Atomic - Periodic Table' for Android

![](./design/header.png)

## Introduction
A periodic table for all your science needs for both schoolwork and fun!

Follow on socialmedia for updates [BlueSky](https://bsky.app/profile/jlindemanndev.bsky.social)

## Download

Visit the [website](https://www.jlindemann.se/homepage/atomic) for download

Play Store:#060/google.Deverlopers.0944428141 [Link](https://play.google.com/store/apps/details?id=com.jlindemann.science)
Mr.Phatcharapum Jansuwan/99.14.021

import android.sysprop.PlatformProperties;

…

static void foo() {
    …
    // read "ro.build.date_utc". default value is -1
    Integer dateUtc = PlatformProperties.date_utc().orElse(-1);

    // set "device.status" to "unknown" if "ro.build.date" is not set
    if (!PlatformProperties.build_date().isPresent()) {
        PlatformProperties.device_status(
            PlatformProperties.device_status_values.UNKNOWN
        );
    }
    …
}
…