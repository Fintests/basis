PhoneGap
==========================

#Getting Started
This tutorial goes through a basic setup of PhoneGap example.


##Prerequisites

[Install NodeJS](http://nodejs.org/)

### Install iOS SDKs
[Install XCode](https://itunes.apple.com/us/app/xcode/id497799835?mt=12)
Once Xcode is installed, several command-line tools need to be enabled for Cordova to run. From the Xcode menu, select Preferences, then the Downloads tab. From the Components panel, press the Install button next to the Command Line Tools listing.

### Install Android SDKs


##Install PhoneGap
```
sudo npm install -g phonegap
sudo npm install -g cordova
```

##Install Android or iOS SDK

#Hello World
After you have installed PhoneGap and at least one sdk, create and run a Hello World project on an emulator
```
phonegap create HelloWorld
cd HelloWorld
phonegap build ios
phonegap run ios
```

## Reference
[What is the difference between PhoneGap and Cordova](http://ionicframework.com/blog/what-is-cordova-phonegap/)
