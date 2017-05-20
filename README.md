# reactNativeAppTutorial
* docs are here: https://facebook.github.io/react-native/docs/tutorial.html
* install: `npm install -g react-native-cli`
* go through the installation files but go here for jdk installation: https://www.digitalocean.com/community/tutorials/how-to-install-java-with-apt-get-on-ubuntu-16-04
* also use this one : http://stackoverflow.com/questions/32942023/ubuntu-openjdk-8-unable-to-locate-package
* install android studio
* extract the zip file and save it here by typing: `sudo mv android-studio /usr/local`
* then go to the folder and type: `cd /usr/local/android-studio/bin`
* then to launch the installer type: `./studio.sh`

## to uninstall android-studio
* go to Home and delete any "Android" things there
* go to /usr/local and type :`rm -rf android-studio`
* To show these hidden folders in the file manager press Ctrl+H when in your home directory (aka "~")
* also remove: `rm -rf ~/.AndroidStudio`
* also remove: `rm -rf ~/.android`
* or just delete it in the folder

## install react native App
* `react-native init testApp`
* `cd testApp`
* `react-native run-android`
