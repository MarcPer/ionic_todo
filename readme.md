# Ionic
Ionic adds front-end functionality to apps built with Cordova or Phone Gap. It is analogous to a Twitter Bootstrap for web applications.


## Get started
Install node, then ionic and cordova:

```bash
sudo apt-get update
sudo apt-get install nodejs
sudo npm install -g ionic cordova
```

Start project and add platform(s)

```bash
ionic start ionic_todo blank
cd ionic_todo
ionic platform add android # can substitute android for ios; requires iOS license (see below)
```

## Ionic View
Ionic View is an app available on the Google Play and Apple App Stores that lets users test an application written with Ionic. The app to be tested is to be added to a remote repository with the following, assuming an Ionic account has already been created:

```bash
ionic login
ionic upload
ionic share email@example.com # optional
```