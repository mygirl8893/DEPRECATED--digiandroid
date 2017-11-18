## DigiByte Android Project

This project is stored in two folders.

digibytej - This is the base Java Library for Digibyte.
digibyte-wallet - This is the Android App
This app was forked originally from the Bitcoin Wallet App. 

## OSX Build Instructions

Install Android Studio
https://developer.android.com/studio/index.html

Install Java JDK
http://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.html

Install Maven
```sh
brew install maven
```

Clone DigiAndroid
```sh
git clone https://github.com/digibyte/digiandroid.git
```

Navigate to DigiBytej Folder
```sh
cd digibytej
```

Make Wallet
```sh
mvn clean install -DskipTests
```

## Checklist
Android sdk and the correct api version installed

Java JDK

Apache maven 3.10?

Clone the digiandroid repo

CD into digibytej
```sh
mvn clean install -DskipTests
```

Cd checkpoints  dir
```sh
mvn exec:java -Dexec.mainClass=com.google.bitcoin.tools.BuildCheckpoints
```



Development was done with IntelliJ IDEA 12.1.4. Open the digibytej project to open all projects with proper linking.

This file system also contains the maven files. They should work correctly but test will fail. append -Dmaven.test.skip=true to the command line.
