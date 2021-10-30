# [Android Fundamentals](https://developer.android.com/guide/components/fundamentals)

* The Android apps can be written using **Kotlin**, **C ++** and **Java** languages.

* An Android package: it is contains an archive file with `.apk` suffix which contains the contents of an Android app that are required at runtime.

* An Android App Bundle: it is an archive with a `.aab` suffix that contains the contents of an Android app project including some additional metadata that is not required at runtime.

Each Android app protected by Android security featurs:

1. The Android operating system.

2. The system sets permissions for all the files in an app so that only the user ID assigned to that app can access them.

3. Each process has its own virtual machine (VM), so an app's code runs in isolation from other apps.

4.  The Android system starts the process when any of the app's components need to be executed, and then shuts down the process when it's no longer needed or when the system must recover memory for other apps.

## App Components

The basic components of any Android application are:

1. **Activities**: An activity represents a single screen with a user interface,in-short Activity performs actions on the screen. 

2. **Services**: A service is a component that runs in the background to perform long-running operations. For example, a service might play music in the background while the user is in a different application.

3. **Broadcast receivers**: Broadcast Receivers simply respond to broadcast messages from other applications or from the system.

4. **Content providers**: A content provider component supplies data from one application to others on request. Such requests are handled by the methods of the ContentResolver class. The data may be stored in the file system, the database or somewhere else entirely.

## The manifest file

Before the Android system can start an app component, the system must know that the component exists by reading the app's manifest file, `AndroidManifest.xml`. In this file, the developer must declare all app components. Also, the manifest does a number of things in addition to declaring the app's components, such as:

1. Identifies any user permissions the app requires, such as Internet access.

2. Declares the minimum API Level required by the app, based on which APIs the app uses.

3. Declares hardware and software features used or required by the app, such as a camera.

4. Declares API libraries the app needs to be linked against (other than the Android framework APIs), such as the Google Maps library.

