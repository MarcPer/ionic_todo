# Ionic
[Ionic](http://ionicframework.com/) adds front-end functionality to apps built with [Cordova](https://cordova.apache.org/) or [PhoneGap](http://phonegap.com/). It is analogous to a [Twitter Bootstrap](http://getbootstrap.com/) for web applications.


## Get started

* Install [nodejs](https://nodejs.org/), then Ionic and Cordova:

```bash
sudo apt-get update
sudo apt-get install nodejs
sudo npm install -g ionic cordova
```

Ionic ships with a CLI. To show all commands type `ionic help` or `ionic --help`.

* Start project and add platform(s)

```bash
ionic start ionic_todo blank
cd ionic_todo
ionic platform add android # can substitute android for ios; requires iOS license (see below)
```

* Build APK (or iOS equivalent) and run it on the web emulator:
```bash
ionic build android
ionic emulate android
```

Alternatively, the app can be tested in the browser with `ionic serve` or on a connected device with `ionic run android`. To test on iOS, an Apple Developer account is needed. Follow instructions from [here](http://ionicframework.com/docs/guide/testing.html). Browser testing is useful for development as the app is updated automatically as soon as the code changes.

## Ionic View
Ionic View is an app available on the Google Play and Apple App Stores that lets users test an application written with Ionic. The app to be tested is to be added to a remote repository with the following, assuming an Ionic account has already been created:

```bash
ionic login
ionic upload
ionic share email@example.com # optional
```