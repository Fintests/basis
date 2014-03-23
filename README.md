PhoneGap
==========================

#Getting Started
This tutorial will guide you through how to setup Cordova (aka PhoneGap) and the [Ionic Framework](http://ionicframework.com) to create a simple ToDo app.

*What is Cordova?*
PhoneGap/Cordova is a simple but powerful API to call Javascript functions that map to native code or plugins. This means you can transfer any kind of data from native land into web land. [Reference](http://ionicframework.com/blog/what-is-cordova-phonegap/)


## Prerequisites
[Install NodeJS](http://nodejs.org/)

Or if you already have node installed, then upgrade to the latest version if you haven't already:
```
sudo npm cache clean -f
sudo npm install -g n
sudo n stable
```

### Install Device SDKs
Install the SDKs for each device you would like your app to run on. If you own a mac, I suggest using iOS SDKs because its significantly quicker to test with the emulator.

#### Install iOS SDKs
[Install XCode](https://itunes.apple.com/us/app/xcode/id497799835?mt=12)
Once Xcode is installed, several command-line tools need to be enabled for Cordova to run. From the Xcode menu, select Preferences, then the Downloads tab. From the Components panel, press the Install button next to the Command Line Tools listing.

#### Install Android SDKs
[Instructions for Android SDK](http://docs.phonegap.com/en/edge/guide_platforms_android_index.md.html#Android%20Platform%20Guide)
The setup for Android SDK is a little more complicated than iOS, follow the instructions in the link above.

### Install Cordova
```
sudo npm install -g cordova
```

## The ToDo App Tutorial
Now that we have all the required software installed, lets get started building our ToDo App!

```
$ git clone xx
$ cordova platform add ios
$ cordova build ios
$ cordova emulate ios
```
Swap ios with android if that's your preferred platform.

http://ionicframework.com/docs/guide/starting.html


###  Cordova Command Line Cheatsheet
```
$ cordova create hello com.example.hello "HelloWorld" -- creates a new cordova app
$ cd hello
$ cordova platform add ios -- adds sdks, can also use add android
$ cordova build ios -- generates platform specific files eg xcodeproj files
$ cordova emulate ios -- runs app on emulator
```

## Reference
[What is the difference between PhoneGap and Cordova](http://ionicframework.com/blog/what-is-cordova-phonegap/)
