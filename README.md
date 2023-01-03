# DISCONTINUATION OF PROJECT #
This project will no longer be maintained by Intel.
Intel has ceased development and contributions including, but not limited to, maintenance, bug fixes, new releases, or updates, to this project.
Intel no longer accepts patches to this project.
Cordova on Android Things allows developers to use standard web
technologies such as HTML5, CSS3, and JavaScript for cross-platform
development. This creates new opportunities for mobile developers as
they now have another platform where they can seamlessly deploy their
applications.

This project will be a repository for sample code that combines Cordova,
plugins and UPM/MRAA for IO programming on Android Things devices. See
also https://github.com/intel-iot-devkit/android-things-samples for more
information on writing UPM/MRAA Java programs for Android Things.

PreRequisites
-------------
1. Follow https://github.com/intel-iot-devkit/android-things-samples#prerequisites for the general Android Thigns environment setup.
2. Install the [Cordova for Android requirements](http://cordova.apache.org/docs/en/latest/guide/platforms/android/index.html)
3. Install the [Cordova command line](http://cordova.apache.org/docs/en/latest/guide/cli/index.html#installing-the-cordova-cli)

Create Android Things Application
---------------------------------
Basically follow the [offical Cordova for Android development cycle](http://cordova.apache.org/docs/en/latest/guide/cli/index.html), just reuse the platform **android**. In longer term, we plan to work with Cordova community to try to add android-things as new platform. Below are typical steps we can use:
```
$ cordova create hello com.example.hello HelloWorld
$ cd hello
$ cordova platform add android
$ cordova build
```

With above steps, you could change files under `www` and call any standard API offer by [WebView](https://developer.android.com/reference/android/webkit/WebView.html). [Mozilla MDN](https://developer.mozilla.org/) and [W3Schools](https://www.w3schools.com/) are good website to learn the APIs. Because of different web engine and version, http://caniuse.com/ can be used to search the API readiness. The Chromium WebView in DP4 is `52.0.2743.100`.

Plugins
-------
Sometimes, the standard Web APIs are not enough especially to access the native components. The cordova plugins can be used which provide JavaScript interface to native components.
```
$ cordova add plugin cordova-plugin-file
```

**NOTE***: Not all Android plugins are promised working on Android Things, please check the [plugin status page](./plugins_status.md)  for details.
