# K-9 Documentation Repo

Documentation for [K-9 Mail](https://k9mail.app/).

Uses [mkdocs](https://www.mkdocs.org/) to generate static HTML.

Changes to the `main` branch are automatically published to the
website using Github Actions.

You can preview local changes using `pip install mkdocs`; `mkdocs serve`,
then visiting http://127.0.0.1:8000/

## Creating Screenshots

For consistency of appearance, we use a virtual device with the following settings for taking screenshots.

* Name: Nexus 5 
* Size: 1080x1920 
* Density: xxhdpi
* API 29 "Android 10.0 (Google APIs)" - not "... (Google Play)"

The Android emulator has a built-in screenshot function, so you do not need crop your desktop.

To take a screenshot use the camera icon on the right of the emulator screen.

![](readme_images/screenshot_icon.png)

The screenshot will be saved in a default location, which can be found in the settings (click
the botton "..." icon, then "Settings" -> "Screenshot Save Location")