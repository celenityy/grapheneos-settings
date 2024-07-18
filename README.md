# grapheneos-settings

My recommendations for the ultimate GrapheneOS Configuration :)

**NOTE:** This project can be found on both [Codeberg](https://codeberg.org/Magnesium1062/grapheneos-settings), which will act as the main & preferred way to contribute, and [GitHub](https://github.com/Retold3202/grapheneos-settings).

# Network & internet

Internet -> **Wi-Fi** -> ❌ *when not using*

Internet -> Network preferences:

* **Turn on Wi-Fi automatically** -> ❌

* **Notify for public networks** -> ❌

* **Turn off Wi-Fi automatically** -> Your choice, the lower the better, I leave mine at `1 minute`

<br>

SIMs -> *Select your carrier* -> **Preferred network type** -> `LTE only`

SIMs -> *Select your carrier* -> **Allow 2G** -> ❌

SIMs -> *Select your carrier* -> **Vo5G** -> ❌

**eSIM support** -> ❌ *if not using*

**Airplane Mode** -> ✅ *when not using cell data*

Hotspot & Tethering:

* **Wi-Fi hotspot** -> ❌

* **USB tethering** -> ❌

* **Bluetooth tethering** -> ❌

* **Ethernet tethering** -> ❌

<br>

VPN -> *Select your VPN if you use one (you should)* -> **Always-on VPN** -> ✅ *(Should be default)*

VPN -> *Select your VPN if you use one (you should)* -> **Block connections without VPN** -> ✅ *(Should be default)*

Private DNS -> **Private DNS provider hostname** -> Pick a private/secure DNS provider of your choice, I would recommend setting up your own [NextDNS](https://nextdns.io) configuration if you are able to (See my recommendations for NextDNS [here](https://codeberg.org/Magnesium1062/nextdns-settings)), otherwise I would recommend [Quad9](https://quad9.net/): `dns.quad9.net`

**Internet connectivity checks** -> `Off` *(You can re-enable when necessary to connect on public networks with captive portals)*

**Attestation key provisioning** -> `GrapheneOS proxy` *(Should be default)*

**Widevine provisoning** -> `GrapheneOS proxy` *(Should be default)*

# Connected devices

Connection preferences:

* Bluetooth -> **Use Bluetooth** -> ❌ *when not using*

* Bluetooth -> **Device name** -> Keep this generic, I recommend setting it to `Device` *(You will need to temporarily turn on Bluetooth for this option to appear, don't forget to disable Bluetooth again after)*

* Bluetooth -> **Turn off Bluetooth automatically** -> Your choice, the lower the better, I leave mine at `1 minute`

* NFC -> **Use NFC** -> ❌ *when not using*

* NFC -> **Require device unlock for NFC** -> ✅ *(You will need to temporarily turn on NFC to toggle this option, don't forget to disable NFC again after)*

* Printing -> Default Print Service -> **Use print service** -> ❌ *if not using* *(Also do the same for your Work profile if you have one)*

* **Ultra-Wideband (UWB)** -> ❌ *(You will need to temporarily turn off Airplane Mode to toggle this option, don't forget to enable Airplane Mode again after)*

# Apps

Go through all apps and remove permissions that are unneeded

I would also recommend removing the `Sensors` permission from `Apps`, `Calculator`, `Clock`, `Contacts`, `Files`, `Gallery`, `Keyboard`, `Messaging`, `PDF Viewer`, `Vanadium`, & `Vanadium System WebView` *(For `Vanadium System WebView` to appear, you must select the 3 dots on the top right corner and select `Show system`)

**App battery usage** -> This is a great option to take advantage of, I would recommend disabling background usage for any apps that don't need to run in the background, as this can heavily improve battery life & privacy. You can also allow unrestricted access here to any apps that do need to run in the background, like Signal or Molly without Google Play.

**Special app access** -> Go through the options here and make sure nothing is granted any of these permissions that doesn't 100% need it

Special app access -> **Special access to hardware accelerators for Google apps** -> `Access not granted` ❌

# Notifications

**App notifications** -> Go through and disable notifications for any apps that don't need it

Notification history -> **Use notification history** -> ❌ *(Should be default)*

**Device & app notifications** -> Make sure this isn't granted to any apps that don't actually need it besides i.e. the launcher

**Notifications on lock screen** -> `Hide silent conversations and notifications`

**Sensitive notifications** -> ❌

**Sensitive work profile notifications** -> ❌

Flash notifications -> **Camera flash** -> ❌ *(Why?)*

Flash notifications -> **Screen flash** -> ❌ *(Why?)*

Wireless emergency alerts:

* **AMBER alerts** -> ❌

* **State and local tests** -> ❌

<br>

**Hide silent notifications in status bar** -> ✅

**Enhanced notifications** -> ❌

# Battery

**Battery percentage** -> ✅

**Battery share** -> ❌

# Display

**Adaptive brightness** -> ❌ *(Annoying and better for battery)*

**Lock screen** -> `Show sensitive content only when unlocked`

**Screen timeout** -> Your choice, the lower the better, I leave mine at `After 1 minute of inactivity`

**Dark theme** -> ✅

Night Light -> **Schedule** -> `Turns on at custom time`

Night Light -> **Start time** -> `9:00 PM`

Night Light -> **End time** -> `6:00 AM`

**Colors** -> `Natural`

**Screen resolution** -> `Full resolution` *(You could set this to `High resolution` if you need to conserve battery)*

**Smooth Display** -> ✅ *(You could disable this if you need to conserve battery)*

**Increase touch sensitivity** -> ✅ *(if you use a screen protector)*

# Wallpaper & style

Lock screen -> More lock screen options:

* **Use device controls** -> ✅ *(harmless)*

* **Dynamic clock** -> ❌

* **Always show time and info** -> ❌

* **Tap to check phone** -> `Off` ❌

* **Lift to check phone** -> `Off` ❌

* **Wake screen for notifications** -> ✅ *(You could disable this if you need to conserve battery)*

* **When work profile is locked** -> `Hide sensitive work content`

<br>

Home screen -> **Themed icons** -> ✅

# Accessibility

Please, please, please, do **NOT** grant any apps the accessibility permission unless you actually need to. This is a very dangerous permission, very concerning from a privacy & security stand-point, please be careful.

# Security

**Screen lock** -> I would recomend using a strong `Password` and avoiding fingerprint, face, or PIN if possible.

Screen lock -> **Lock after screen timeout** -> Your choice, the lower the better, I leave mine at `5 seconds after timeout`

Screen lock -> **Power button instantly locks** -> ✅

**Auto reboot** -> Your choice, the lower the better, I leave mine at `8 hours`

**Duress password** -> This is a great setting, make sure to enable and take advantage of it.

**USB peripherals** -> `Allow new USB peripherals when unlocked` *(If you don't use any USB devices at all with your device, you should set this to `Disallow new USB peripherals`)*

**USB-C port** -> `Charging-only when locked` *(If you don't use any USB devices at all with your device, you should set this to `Charging-only`)*

Secure app spawning -> **Use secure app spawning** -> `Enabled` ✅

**Automatic exploit protection compatibility mode** -> ❌ *(If you're not willing to troubleshoot the very rare times an app has issues, then you could potentially leave this on)*

Native code debugging -> **Block for third-party apps by default** -> ✅

**Scramble PIN input layout** -> ✅

**Allow camera access when the device is locked** -> ❌

**Notify about system process crashes** -> ✅

More security settings:

* **Device admin apps** -> Go through and remove this permission from any apps that don't absolutely need it

* SIM lock -> **Lock SIM** -> ✅ *(You might have to find your carrier's default SIM PIN)*

* Encryption & credentials -> Trusted credentials -> **User** -> Remove any certificates you don't need/use

* Encryption & credentials -> **User credentials** -> Remove any certificates you don't need/use

* Work profile security -> **Use one lock** -> ✅

* **Fingerprint unlock for work** -> ❌ *(You should use a strong password instead)*

# Privacy

**Camera access** -> ❌ *when not using*

**Microphone access** -> ❌ *when not using*

**Allow Sensors permission to apps by default** -> ❌

**Save screenshot timestamp to EXIF** -> ❌

**Show passwords** -> ❌

**Show media on lock screen** -> ✅ *(harmless)*

**Show clipboard access** -> ✅

# Location

**Use location** -> ❌ *when not using*

Location services -> **Wi-Fi scanning** -> ❌ *(Should be default, make sure to also set for your `Work` profile if you have one)*

Location services -> **Bluetooth scanning** -> ❌ *(Should be default, make sure to also set for your `Work` profile if you have one)*

SUPL is used to speed-up acquiring location, but it comes at the cost of potentially sending sensitive information to Google, such as your MCC, MNC, nearby cell towers, and the strength of those towers. While GrapheneOS does proxy this connection, which helps to improve privacy, this is still not ideal, as Google is still sent this data. I have personally not noticed any difference acquiring location with this off, so as long as you're on a newer Pixel, I would highly recommend just disabling this. You can read more about SUPL, as well as PSDS [here](https://divestos.org/misc/gnss.txt):

**Secure User Plane Location (SUPL)** -> `Off`

**Predicted Satellite Data Service (PSDS)** -> `GrapheneOS server` *(harmless)*

# System

Keyboard -> On-screen keyboard -> Keyboard:

* Preferences -> **Auto-capitalization** -> ❌

* Preferences -> **Voice input key** -> ❌ *if you don't use*

* Text correction -> **Block offensive words** -> ❌

* Text correction -> **Personalized suggestions** -> ❌ *(Should be default)*

* Text correction -> **Suggest Contact names** -> ❌

* Advanced -> **Emoji for physical keyboard** -> ✅

<br>

Keyboard -> Spell checker -> **Look up contact names** -> ❌

Gestures -> **Navigation mode** -> ✅ `Gesture navigation` *(I held out on `3-button navigation` for ages, but after finally switching, I can say it's a game-changer, so much better, please try it)*

Gestures -> Navigation mode -> Gesture navigation -> **Swipe to invoke assistant** -> ❌

Gestures -> Navigation mode -> 3-button navigation -> **Hold home for assistant** -> ❌

Date & time -> **Set time automatically** -> ✅ *This is very important for security*

Date & time -> Time zone -> **Set automatically** -> ✅

Date & time -> Time format -> **Use 24-hour format** -> ❌

System updates -> **Release channel** -> `Stable` *(Should be default)*

System updates -> **Permitted Networks** -> `Any` *(Should be default)*

System updates -> **Require battery above warning level** -> ✅

System updates -> **Require device to be charging** -> ❌ 

System updates -> **Automatic Reboot** -> ❌ *(Should be default, I found this way too annoying)*

# Developer options

**OEM unlocking** -> ❌

**Automatic system updates** -> ✅ *(Should be default)*

**USB debugging** -> ❌ *when not using*

**Wireless debugging** -> ❌ *when not using*

**Logger buffer sizes** -> `Off`

**Force peak refresh rate** -> ✅ *(You could disable this if you need to conserve battery)*

**Wi-Fi Scan Throttling** -> ✅ *(Should be default)*

**Mobile data always active** -> ❌

**Window animation scale** -> `.5x`

**Transition animation scale** -> `.5x`

**Animator duration scale** -> `.5x`

**Allow window-level blurs** -> ❌

**Always show crash dialog** -> ✅

**Suspend execution for cached apps** -> `Enabled`

**Force allow apps on external** -> ✅

**Predictive back animations** -> ✅

# About phone

**Device name** -> Keep this generic, I recommend setting it to `Device`