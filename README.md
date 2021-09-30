# ArmBot_Javascript
This project aims to focus on the HMI of the ArmBot. HMI is a web app, developped in the Javascript language, using **Cordova** framework in order to build for both **Android** and **IOS**.

# Prerequisites
**NodeJS** is mandatory in order to use **Apache Cordova** framework.

Basic knowledge of Javascript and OOP.

# Install NodeJS and Cordova library
1. Download and install [Node.js](https://nodejs.org/en/download/). On installation you should be able to invoke **node** and **npm** on your command line.
2. Download and install a [git client](http://git-scm.com/downloads), if you don't already have one. Following installation, you should be able to invoke **git** on your command line.
3. Install the **Cordova** module using **npm** utility of Node.js. The cordova module will automatically be downloaded by the npm utility.
* On OS X and Linux

`sudo npm install -g cordova`

On OS X and Linux, prefixing the npm command with sudo may be necessary to install this development utility in otherwise restricted directories such as /usr/local/share. If you are using the optional nvm/nave tool or have write access to the install directory, you may be able to omit the sudo prefix. There are more tips available on using npm without sudo, if you desire to do that.

* On Windows

`C:\>npm install -g cordova`

The -g flag above tells npm to install cordova globally. Otherwise it will be installed in the node_modules subdirectory of the current working directory.

# Create the App
1. Clone this repository

`git clone https://github.com/ArmBot-ECE/ArmBot_Javascript.git`

2. Go in this directory

`cd ArmBot_Javascript`

3. Install all dependancies
**Cordova** uses NodeJS modules to add extra features. All modules are stored in `node_modules` folder and listed in config file `package.json`. **Never push this folder on GitHub**, config file `package.json` is there to install all dependancies when setting up the app.

4. Go to child folder `ArmBot_Javascript`

`cd ArmBot_Javascript`

5. Install all dependancies listed in config file `package.json`

`npm install`

6. Using your favorite IDE, you can code in `www` folder.

Only work done in this folder and config files `config.xml` `package.json` must be pushed on this repository.



