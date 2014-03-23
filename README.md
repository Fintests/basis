PhoneGap
==========================

#Getting Started
This tutorial goes through a basic setup of PhoneGap/Cordova example.


###Prerequisites
[Install NodeJS](http://nodejs.org/)
Or if you already have node installed, then upgrade to the latest version if you haven't already:
```
sudo npm cache clean -f
sudo npm install -g n
sudo n stable
```

#### Install iOS SDKs
[Install XCode](https://itunes.apple.com/us/app/xcode/id497799835?mt=12)
Once Xcode is installed, several command-line tools need to be enabled for Cordova to run. From the Xcode menu, select Preferences, then the Downloads tab. From the Components panel, press the Install button next to the Command Line Tools listing.

#### Install Android SDKs
[Instructions for Android SDK](http://docs.phonegap.com/en/edge/guide_platforms_android_index.md.html#Android%20Platform%20Guide)
The setup for Android SDK is a little more complicated than iOS, follow the instructions in the link above.

####Install Cordova
```
sudo npm install -g cordova
```

###  A Hello World Example
```
$ cordova create hello com.example.hello "HelloWorld"
$ cd hello
$ cordova platform add ios
$ cordova build
$ cordova run ios
```


## Reference
[What is the difference between PhoneGap and Cordova](http://ionicframework.com/blog/what-is-cordova-phonegap/)
