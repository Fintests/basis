Cordova / PhoneGap
==========================

#Getting Started
This tutorial will guide you through how to setup Cordova (aka PhoneGap) and the [Ionic Framework](http://ionicframework.com) to create a simple ToDo app.

#####What is Cordova?
PhoneGap/Cordova is a simple but powerful API to call Javascript functions that map to native code or plugins. This means you can transfer any kind of data from native land into web land. [Reference](http://ionicframework.com/blog/what-is-cordova-phonegap/)

## ToDo App
* follow tutorial to build basic todo app
* add some RESTful web services in any language which store tasks in monogoDB
* deploy web services to heroku
* update app to call webservices

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
$ sudo npm install -g cordova
```

### Hello World Cordova
Create a simple hello world app to test its all working. The emulator make take a bit of time to start up for the first time.

You should see the Cordova logo and "Device is Ready" displayed on the emulate.

```
$ cordova create helloWorld
$ cordova platform add ios
$ cordova build ios -- swap with android if required
$ cordova emulate ios
```
At this point we have our device SDK + Cordova installed. The next step is to install the Ionic Framework and begin with the ToDo tutorial.

## Installing Ionic & The ToDo App Tutorial
Now that we have all the required software installed, lets get started building our ToDo App with Ionic!

Great! You should have a very basic Corodva app up and running, now lets turn it into a ToDo app by working our way through the Ionic Guid [here](http://ionicframework.com/docs/guide/starting.html).

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


# Updates to the tutorial
## ionic.css

Change
```
<link href="lib/ionic/css/ionic.css" rel="stylesheet">
```
to
```
<link href="css/ionic.css" rel="stylesheet">
```
Make a new file in `www/js` called `ionic.css`. Copy all the code from [ionic.css](https://raw.githubusercontent.com/driftyco/ionic/master/release/css/ionic.css) into your new file.

## ionic.bundle.js

Change
```
<link href="lib/ionic/js/ionic.bundle.js" rel="stylesheet">
```
to
```
<link href="lib/ionic/js/ionic.bundle.js" rel="stylesheet">
```
Make a new file in `www/js` called `ionic.bundle.js`. Copy all the code from [ionic.bundle.js](https://raw.githubusercontent.com/driftyco/ionic/master/release/js/ionic.bundle.js) into your new file.
