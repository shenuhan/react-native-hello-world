# react-native-hello-world

first install a JDK >= 17
and node >= 22

# install android studio ou android sdk

ubuntu : 
    sudo snap install androidsdk
    androidsdk 'build-tools;36.0.0'
    androidsdk 'platforms;android-36'
    androidsdk 'cmdline-tools;latest'
    androidsdk 'platform-tools'
windows : 
    https://developer.android.com/studio?hl=fr
    installer les package avec le package manager

créé une variable environement 
windows : ANDROID_HOME -> C:\Users\<username>\AppData\Local\Android\Sdk\
ubuntu : ANDROID_HOME=~/AndroidSDK/ <- le / a la fin est important

Ajouté au path $ANDROID_HOME/emulator et $ANDROID_HOME/platform-tools

# run on android
adb devices doit afficher le device
(debugger option sur le tel, moi j'ai fais en wifi)
Wifi : 
 tel: click pair sur debug option wifi
 pc: adb pair <ip>:<pairing_port>
 pc : adb connect <ip>:<connect_port>

npx expo install expo-dev-client
npx expo run:android