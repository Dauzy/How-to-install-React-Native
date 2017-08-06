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
Note: If you have permission errros to install utility check here.

# Fixing npm permissions
#### 1. First find the path to npm's directory
```
$ npm config get prefix
```
#### 2. Change the owner of npm's directories to the name of the current user (your username!):
```
$ sudo chown -R $(whoami) $(npm config get prefix)/{lib/node_modules,bin,share}
```
