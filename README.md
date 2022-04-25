# K-9 Mail User Manual

This repository is the home of the user documentation for [K-9 Mail](https://k9mail.app/). Contributions are welcome.

Uses [mkdocs](https://www.mkdocs.org/) to generate static HTML.

Changes to the `main` branch are automatically published to the website using GitHub Actions.

## Building the Site

You can preview local changes using `pip install mkdocs-material mkdocs-redirects`; `mkdocs serve`,
then visiting http://127.0.0.1:8000/

## Creating Screenshots

For consistency of appearance, we use a virtual device with the following settings for taking screenshots.

* Name: Pixel 2
* Size: 1080x1920 
* Density: 420 dpi
* API 31 "Android 12.0 (Google APIs)" - not "… (Google Play)"

Follow the [System UI Demo Mode](https://android.googlesource.com/platform/frameworks/base/+/master/packages/SystemUI/docs/demo_mode.md)
activation instructions:

```
adb shell settings put global sysui_demo_allowed 1     # only needed once
adb shell am broadcast -a com.android.systemui.demo -e command enter
adb shell am broadcast -a com.android.systemui.demo -e command clock -e hhmm 1200
adb shell am broadcast -a com.android.systemui.demo -e command network -e wifi show -e level 4
adb shell am broadcast -a com.android.systemui.demo -e command network -e mobile show -e level 4 -e datatype lte
adb shell am broadcast -a com.android.systemui.demo -e command battery -e level 100 -e plugged false
adb shell am broadcast -a com.android.systemui.demo -e command notifications -e visible false
```

To take a screenshot click the camera icon next to the emulator window.

![Android emulator with toolbar window](readme_images/screenshot_icon.png)

Newer version of Android Studio prompt you for a location to save.

Otherwise the screenshot will be saved in a default location, which can be found in the settings (click
the bottom "..." icon, then "Settings" -> "Screenshot Save Location")
