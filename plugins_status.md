This page summarize the readniess of Codova 7.x plugins for [Android Things on Intel® Joule™](https://developer.android.com/things/hardware/joule.html) **Developer Preview release 4**.

Basically, Android mobile plugins are re-used as much as possible for Android Tings platform. Some are working without any change, some are required patches(will upstream), and some are newly developed plugins(will open source).

* Existing plugins w/o any changes, just follow normal [add plugins](http://cordova.apache.org/docs/en/latest/guide/cli/index.html#add-plugins) steps:
```
cd <your_cordova_app_dir>
cordova plugin add <plugin_name>

```

* Existing plugins need patch or new plugins
```
cd <your_cordova_app_dir>
cordova plugin add <plugin_repo_with_patch>

```

Cordova 7.x official plugins
-------------
| Plugin | Status | Repo URL if need patch | Comment |
|--------|--------|------------------------|---------|
| [Battery Status](http://cordova.apache.org/docs/en/latest/reference/cordova-plugin-battery-status/index.html)           | Verified on AC |  | No battery on Joule |
| [Console](http://cordova.apache.org/docs/en/latest/reference/cordova-plugin-console/index.html)                         | Verified |  |  |
| [Device](http://cordova.apache.org/docs/en/latest/reference/cordova-plugin-device/index.html)                           | Verified |  |  |
| [Dialog](http://cordova.apache.org/docs/en/latest/reference/cordova-plugin-dialogs/index.html)                          | Verified |  |  |
| [InAppBrowser](http://cordova.apache.org/docs/en/latest/reference/cordova-plugin-inappbrowser/index.html)               | Verified |  |  |
| [Splashscreen](http://cordova.apache.org/docs/en/latest/reference/cordova-plugin-splashscreen/index.html)               | Verified |  |  |
| [File](http://cordova.apache.org/docs/en/latest/reference/cordova-plugin-file/index.html)                               | Verified |  |  |
| [Globalization](http://cordova.apache.org/docs/en/latest/reference/cordova-plugin-globalization/index.html)             | Verified |  |  |
| [Whitelist](http://cordova.apache.org/docs/en/latest/reference/cordova-plugin-whitelist/index.html)                     | Verified |  |  |
| [Network Infromation](http://cordova.apache.org/docs/en/latest/reference/cordova-plugin-network-information/index.html) | Verified |  |  |
| [File Transfer](http://cordova.apache.org/docs/en/latest/reference/cordova-plugin-file-transfer/index.html)             | Verified |  |  |
| [Vibration](http://cordova.apache.org/docs/en/latest/reference/cordova-plugin-vibration/index.html)                     | Verified | [https://github.com/fujunwei/cordova-plugin-vibration](https://github.com/fujunwei/cordova-plugin-vibration/tree/android_things) |  |
| [Device Motion](http://cordova.apache.org/docs/en/latest/reference/cordova-plugin-device-motion/index.html)             | Verifed | [https://github.com/fujunwei/cordova-plugin-device-motion](https://github.com/fujunwei/cordova-plugin-device-motion/tree/android_things)  |  |
| [Device Orientation](http://cordova.apache.org/docs/en/latest/reference/cordova-plugin-device-orientation/index.html)   | WIP | N/A  |  |
| [Geolocation](http://cordova.apache.org/docs/en/latest/reference/cordova-plugin-geolocation/index.html)                 |  WIP |  N/A  | |
| [Media](http://cordova.apache.org/docs/en/latest/reference/cordova-plugin-media/index.html)                             | Verifed |  | Play back audio files on a device with SW codec only |
| [Camera](http://cordova.apache.org/docs/en/latest/reference/cordova-plugin-camera/index.html)                           | WIP? | N/A |  |
| [Media Capture](http://cordova.apache.org/docs/en/latest/reference/cordova-plugin-media-capture/index.html)             | Wait for native support | N/A |  |
| [Contacts](http://cordova.apache.org/docs/en/latest/reference/cordova-plugin-contacts/index.html) | Won't suppot | N/A |  |
| [Statusbar](http://cordova.apache.org/docs/en/latest/reference/cordova-plugin-statusbar/index.html) | Won't suppot | N/A |  |

Newly created (private)
-------------
| Plugin | Status | Repo URL | Comment |
|--------|--------|----------|------|
| LED | Verified | [https://github.com/01org/cordova-plugin-led](https://github.com/01org/cordova-plugin-led) |  |
| Temperature | WIP | [https://github.com/01org/cordova-plugin-temperature](http://github.com/01org/cordova-plugin-temperature) |  |
| Humidity | Not started | [https://github.com/01org/cordova-plugin-humidity](http://github.com/01org/cordova-plugin-humidity) |  |
| Air Pressure | Not started | [https://github.com/01org/cordova-plugin-air-pressure](http://github.com/01org/cordova-plugin-air-pressure) |  |
| Air Quality | Not started |  [https://github.com/01org/cordova-plugin-air-quality](http://github.com/01org/cordova-plugin-air-quality) |  |
| Infrared Temperature | Not started | [https://github.com/01org/cordova-plugin-infrared-temperature](http://github.com/01org/cordova-plugin-infrared-temperature) |  |

* If you need permission, please contact Balestrieri, Francesco <francesco.balestrieri@intel.com>
* For those does not listed here but can be searched on https://cordova.apache.org/plugins/, you're welcome to submit Pull Request.
