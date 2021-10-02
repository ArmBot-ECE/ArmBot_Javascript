# ArmBot_Javascript
This project aims to focus on the HMI of the ArmBot. HMI is a web app, developped in the Javascript language, using **Cordova** framework in order to build for both **Android** and **IOS**.

# Prerequisites
**JDK8**.
**NodeJS** is mandatory in order to use **Apache Cordova** framework.

**Android Studio** for **SDK manager**.

**Gradle**

Basic knowledge of Javascript and OOP.

# Install JDK8
1. Check if you have a JDK version 8+ installed on your machine by running command `java -version`
2. If none is installed or you want to install a proper JDK8 with a commercial license, go online, you'll find plenty of tutorials.
3. Don't forget to setup your JRE_HOME and JAVA_HOME environment variables.

# Install NodeJS and Cordova library
1. Download and install [Node.js](https://nodejs.org/en/download/). On installation you should be able to invoke **node** and **npm** on your command line.

For CentOS: [Installation guide](https://matthiashoys.wordpress.com/2020/01/15/how-to-upgrade-node-js-from-v6-to-v12-on-centos-linux-7/)

2. Download and install a [git client](http://git-scm.com/downloads), if you don't already have one. Following installation, you should be able to invoke **git** on your command line.
3. Install the **Cordova** module using **npm** utility of Node.js. The cordova module will automatically be downloaded by the npm utility.
* On OS X and Linux

`sudo npm install -g cordova`

On OS X and Linux, prefixing the npm command with sudo may be necessary to install this development utility in otherwise restricted directories such as /usr/local/share. If you are using the optional nvm/nave tool or have write access to the install directory, you may be able to omit the sudo prefix. There are more tips available on using npm without sudo, if you desire to do that.

* On Windows

`C:\>npm install -g cordova`

The -g flag above tells npm to install cordova globally. Otherwise it will be installed in the node_modules subdirectory of the current working directory.

# Install Gradle
Download the latest [Gradle](https://gradle.org/releases/) distribution

* On Windows
1. Unpack the distribution Create a new directory `C:\Gradle` with File Explorer.

Open a second File Explorer window and go to the directory where the Gradle distribution was downloaded. Double-click the ZIP archive to expose the content. Drag the content folder `gradle-[VERSION]` to your newly created C:\Gradle folder.

Alternatively you can unpack the Gradle distribution ZIP into `C:\Gradle` using an archiver tool of your choice.

2. Configure your system environment
In File Explorer right-click on the This PC (or Computer) icon, then click *Properties -> Advanced System Settings -> Environmental Variables*.
Under System Variables select Path, then click Edit. Add an entry for `C:\Gradle\gradle-4.1\bin`. Click OK to save.

3. Verify your installation
Open a console (or a Windows command prompt) and run below command to run Gradle and display the version, e.g.:

`gradle -v`

* On Linux & MacOS

1. Unzip the distribution zip file in the directory of your choosing, e.g.:
```
mkdir /opt/gradle
unzip -d /opt/gradle gradle-7.2-bin.zip
ls /opt/gradle/gradle-7.2
```

2. Configure your PATH environment variable to include the bin directory of the unzipped distribution, e.g.:
Open your `.bashrc` file, and write this line:
`export PATH=$PATH:/opt/gradle/gradle-4.1/bin`

For OS X you might need to do: `export PATH=$PATH:/opt/gradle/gradle-4.1/bin` in a terminal.

# Instal SDKmanager
* On Linux & MacOS
1. Create directory `android` in `/opt/`
2. Install **Command line tools only** from [Android SDK Downloads](https://developer.android.com/studio/#downloads) in `/opt/android/`
3. Create directory `latest` in `/opt/android/cmdline-tools/`
4. Move folder `bin`, `lib` and files `NOTICE.txt`, `source.properties` in folder `/opt/android/cmdline-tools/latest`
5. **(Optional)** Install **Platform tools** from [Android Platform tools Downloads](https://developer.android.com/studio/releases/platform-tools) in `/opt/android/`
6. Setup **ANDROID_SDK_ROOT** as `/opt/android/`
7. Add to **PATH** `$ANDROID_SDK_ROOT/cmdline-tools/latest/bin`
8. Test install by running `sdkmanager --version`

* On Windows
Part coming...

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



