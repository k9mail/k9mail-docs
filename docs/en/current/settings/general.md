# General Settings 

*General settings* are account-independent settings. Most of them define how the user interface looks.

![General Settings menu](img/settings_general.png)

## Display
The Display settings control the general appearance of the app, as well as each of the 
main views, such as the account list, message lists and message display.

### Global 

#### Language
By default K-9 Mail displays the user interface in the language you're using for your Android system. With this 
setting you can override the system language, e.g. if your Android version doesn't support your native language but 
K-9 Mail does.

#### Theme
Available themes:

* Light
* Dark
* Use system default

#### Fixed message theme
When using the dark theme messages can look wrong. This is why K-9 Mail allows you to override the app theme.

Enabling this setting means K-9 always uses the theme configured in *Message view theme* below for the message view.
Not using a fixed message theme means you can select a theme in the menu of the message view.

#### Message view theme
This setting specifies the theme that is used for the message view.

Available settings:

* Light
* Dark
* Use app theme (default)

#### Composer theme
This setting specifies the theme that is used when composing a message.

Available settings:

* Light
* Dark
* Use app theme (default)

#### Font size

K-9 allows you to configure the font-size for various sections of the app.

The "Message body" slider is a percentage, default 100%.

#### Animation

Currently this only affects the animation when switching from the message list to the message view and back.

### Account List

#### Show Unified Inbox

This shows the Unified Inbox as the first item in the main application drawer. (Enabled by default)

#### Show starred count

Each folder and account always shows the count of unread messages. This option shows also the count of starred messages.

### Message lists

#### Preview Lines

Configures how many lines of each message to show when previewing them in a list. More preview lines mean
fewer messages can be shown at any one time.

#### Show stars

If you do not "star" messages you can disable the icon here to save space.

#### Show correspondent names

Show the sender's name from the email headers rather than the email address.

#### Correspondent above subject

Self-explanatory.

#### Show contact names

If contacts are found in Android's address book, choosing this option means K-9 shows the name from there instead
of from the email itself.

#### Colorize contacts

Show contacts that you already know in a different color. Only available when "Show contact names", above, is selected.

#### Contact name color

Choice of colour for the above option "Colorize contacts".

#### Show contact pictures

Disable this if you don't want to display contact pictures (or place holder images) in the message list.

#### Colorize missing contact pictures

If a contact does not have a picture, K-9 will create a "random" color for the contact based on their email address
that will remain constant. If this is disabled the images will be displayed with a grey background.

#### Change colour when read

Self-explanatory.

### Folder lists

#### Wrap long folder names
When this setting is enabled folder names that are longer than can be displayed in one line in the folder list will be 
wrapped and displayed using multiple lines rather than being shortened with "..."

### Message lists

#### Preview lines
Here you can specify how many lines of preview of a message you want to see in the message list.

**Note:** If you set preview lines to *0* and disable contact pictures (see below) you get a special single line 
message list view.

#### Multi-select checkboxes
Enable this to always show the checkboxes to select a message.

#### Dim messages after reading
Disabling this will display read and unread messages using the same background color in the message list. Then bold 
text in the first line is the only indicator that a message hasn't been read yet.

#### Threaded view
Threaded view is enabled by default and groups messages that belong to the same thread. Currently only messages in the 
same folder are grouped. Specifically, this will not include messages sent by you if those messages are not also stored 
in the current folder.

Please note that this is not the same as the conversation view you might know from e.g. Gmail. 

To add own messages in threaded view: change *Sent folder* to *INBOX* in *Folder* settings under *Account settings*. 

Note: own messages are no longer stored (and synced) in *Sent* folder.

#### Show split-screen
This setting allows you to display the message list next to the message view. This is mainly useful for devices with a 
rather large screen, i.e. tablets.

Available settings:

* Always
* Never
* When in Landscape orientation


### Fixed-width fonts
When this is checked a fixed-width font will be used for plain text messages. The display of HTML messages is not 
influenced by this setting.

#### Visible message actions
Configure which message actions will be promoted to the first level of the menu in the message view.

**Note:** Checking an item doesn't mean that this action will be displayed in the action bar. There is only a limited 
number of actions that will be displayed in the action bar, the rest will move to the so called overflow menu that is 
accessible using the icon with the three dots.

### Messages

#### Auto-fit message
Enable this to shrink messages to fit the screen width.


### Interaction

####  Start in Unified Inbox
When this setting is enabled K-9 Mail starts in the *Unified Inbox*.

**Note:** You shouldn't use this setting. Pressing the launcher icon when K-9 Mail has been started before will restore 
the app to its old state rather than starting it again. Put a "K-9 Accounts" shortcut on your home screen to always 
open the *Unified Inbox*.

### Interaction/Gestures
**Note:** This setting isn't currently used and will be removed soon.

### Interaction/Volume key navigation
Here you can specify whether you want to use the hardware volume keys to move up and down in the message list, or move 
to the previous and next message in the message view.

### Interaction/Return to list after delete
When this setting is enabled deleting a message in the message view will return to the message list rather than moving 
to the previous/next message.

### Interaction/Show next message after delete
Enabling this setting always moves to the next message after deleting a message from the message view. When it is 
disabled you move to the next or previous message depending on your previous travel direction.

### Interaction/Confirm actions
Here you can specify which actions should display a confirmation dialog.

You can enable confirmations for the following actions:

* Delete (in message view)
* Delete Starred (in message view)
* Delete (from notification)
* Spam


## Notifications

Only some options relating to notifications are shown here.
Most of the settings for notifications are under [Account Settings](account.md#notifications), which means you can 
choose different notification styles for each account.
 
### Quiet Time
You can set a *Quiet Time* to prevent notification from disturbing your sleep.

### Quiet Time starts
Here you can specify the time when notifications will be disabled.

### Quiet Time ends
This time specifies the end of the *Quiet Time*, when notifications will be enabled again.

### Show 'Delete' button
K-9 Mail supports deleting messages directly from a notification (on Android 4.1 and newer).

The available settings are:

* Never (default)
* For single message notifications
* Always


## Network

### Background sync
This setting specifies when K-9 Mail is allowed to synchronize messages in the background.

Available settings are:

* When 'Auto-sync' is checked (see below)
* Always
* Never (This disables mail checking for all accounts regardless of the account settings)

'Auto-sync' is an Android-wide setting that controls accounts that link into the phone. Currently K-9 email accounts do 
not function in this way. However setting this will make the app reflect the general auto-sync setting.

The configuration of Android's Auto-sync setting may vary depending on your phone's Android version and device 
manufacturer. On stock Android it's found under: "Settings -> Users & accounts -> Automatically sync data"

* [Google provide information about auto-sync and Nexus phones](https://support.google.com/nexus/answer/2840875?hl=en-GB)
* [Samsung provide instructions for their S6 phones.](https://www.samsung.com/hk_en/support/skp/faq/1075415)
* [On a technical level this is the result from `ContentResolver.getMasterSyncAutomatically()`](https://developer.android.com/reference/android/content/ContentResolver.html#getMasterSyncAutomatically())


## Miscellaneous

### Use Gallery bug work-around
An old Android version shipped with a faulty Gallery app that didn't show any selectable items. To work around this 
bug K-9 Mail adds the options "Add image" and "Add video" to the menu of the message composition screen when this 
setting is enabled.

**Note:** This setting should be automatically enabled when the faulty Gallery version is found on your device. Most 
users can ignore this setting and leave it unchecked.


### Save attachments to...
Here you can specify a directory where your attachments are saved to when the "Save" button of an attachment is clicked.
If a compatible file manager is installed 
(e.g. [OI File Manager](https://play.google.com/store/apps/details?id=org.openintents.filemanager)) you can simply 
select a directory. Otherwise you'll have to type in its name.


## Privacy

### Hide subject in notifications
This setting allows you to hide the subject of a message in notifications.

Available options:

* Never (default)
* When device is locked
* Always


**Note:** Currently, any value other than *Never* disables rich notifications (on Android versions that support them). 
This behavior will most likely change in the future to only disable the notification ticker that is visible from the 
lock screen.


## Debugging

### Enable debug logging
Here you enable the logging of extra diagnostic information – e.g. if you're working with a developer to troubleshoot 
a problem. See the page on [logging errors](../misc/debugging.md) for more information.

Remember to disable debug logging once it's no longer required.

### Log sensitive information
By default, sensitive information like passwords are not saved in the logs, but this option enables logging of 
sensitive information.
