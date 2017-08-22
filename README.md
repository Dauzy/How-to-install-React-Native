# How to install React-Native on Ubuntu 16.04 LTS

First install nodejs, We install nodejs lts 6.x release.

```
$ sudo apt-get install python-software-properties
$ curl -sL https://deb.nodesource.com/setup_6.x | sudo -E bash -
```

Install nodejs
```
$ sudo apt-get install nodejs
```

## 1. Install react-native
We can use npm to install the ```create-react-native-app``` commnad line utility.
```
$ npm install -g create-react-native-app
```
Note: If you have permission errros to install utility check [here](https://gist.github.com/Dauzy/ccc46f72028e121bb67462173971cfeb).

React Native requires a recent version of JDK and Android Studio Environment

## 2. Configure your ANDROID_HOME
React native tools requires some environment variables to build app with native code. You can add some lines to your ```~/.bash_profile``` or ```~/.bashrc```.
```
export ANDROID_HOME=$HOME/Android/Sdk
export PATH=$PATH:$ANDROID_HOME/tools
export PATH=$PATH:$ANDROID_HOME/platform-tools
```
Type ```source ~/.bash_profile``` or ```source ~/.bashrc``` to load config into your current shell.

## 3. Run your first App!
We can uses react-native command line tools to generate a new project.
```
react-native init HelloWorld
```
enter to your project folder and run App
```
cd HelloWorld
npm start
react-native run-android
```

![react-native App](https://raw.githubusercontent.com/Dauzy/How-to-install-React-Native/master/image.png)
