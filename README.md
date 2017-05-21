# reactNativeAppTutorial
* docs are here: https://facebook.github.io/react-native/docs/tutorial.html
* install: `npm install -g react-native-cli`
* go through the installation files but go here for jdk installation: https://www.digitalocean.com/community/tutorials/how-to-install-java-with-apt-get-on-ubuntu-16-04
* type: `sudo apt-get install default-jre`
* type: `sudo apt-get install default-jdk`
* type: `sudo add-apt-repository ppa:webupd8team/java`
* type: `sudo apt-get update`
* type: `sudo apt-get install oracle-java8-installer`
* to check which installation you've got check: `update-java-alternatives --list`

### Setting the JAVA_HOME variable
* find out where java is installed: `sudo update-alternatives --config java`
* Copy the path from your preferred installation, example: `/usr/lib/jvm/java-8-openjdk-amd64/jre/bin/java`
* Also type: `sudo nano /etc/environment`
* add a new line and copy this and save it: `JAVA_HOME="/usr/lib/jvm/java-8-openjdk-amd64/jre/bin/java"`
* reload it by typing: `source /etc/environment`
* test whether it worked by typing: `echo $JAVA_HOME`

# continue with the android studio installation
* download android-studio
* extract the zip file and save it here by typing: `sudo mv android-studio /usr/local`
* then go to the folder and type: `cd /usr/local/android-studio/bin`
* then to launch the installer type: `./studio.sh`
* select "manual"
* select all the options including virtual machine
* install KVM: https://www.cyberciti.biz/faq/installing-kvm-on-ubuntu-16-04-lts-server/
* type: `sudo apt-get install qemu-kvm libvirt-bin virtinst bridge-utils cpu-checker`
* check if its ok, type: `kvm-ok`

## to uninstall android-studio
* go to Home and delete any "Android" things there
* go to /usr/local and type :`rm -rf android-studio`
* To show these hidden folders in the file manager press Ctrl+H when in your home directory (aka "~")
* also remove: `rm -rf ~/.AndroidStudio`
* also remove: `rm -rf ~/.android`
* or just delete it in the folder

## Sdk location not found
* inside your app folder go to the android folder
* create a file called: local.properties
* to find the location of the sdk file open the android-studio, go to configure, sdk manager
* you'll find it there.
* inside the file add the following: `sdk.dir = /home/amv/Android/Sdk`
* see : http://stackoverflow.com/questions/41890659/errorthe-sdk-build-tools-revision-23-0-3-is-too-low-for-project-app-minim
* `export PATH="/home/amv/Android/Sdk/platform-tools":$PATH`

## install react native App
* `react-native init testApp`
* `cd testApp`
* `react-native run-android`
