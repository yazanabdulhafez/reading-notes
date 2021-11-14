# Android

## Application Fundamentals

* Android apps can be written using Kotlin, Java, and C++ languages.
* The Android SDK tools compile  codewith any onther data into an APK or an Android App Bundle.
* An Android package, which is an archive file with an .apk suffix, contains the contents of an Android app required at the runtime.
* An Android App Bundle, which is an archive file with an .aab suffix, contains the contents of an Android app project including some additional metadata that is not required at runtime.
* An AAB is a publishing format and cant be installed on Android devices.

* Each android app is live in its own security sand box and protected by the following featuers offerd by android:

1. The oprating system in android is milti-user linux system.
2. The system assign each user a unique Linux user ID.
3. Each process has its own virtual machine.
4. Every app runs in its own Linux process.

## App components

There are four different types of app components:

1. Activities
2. Services
3. Broadcast receivers
4. Content providers

### Activities

It is the entry point to enteract with the user.

### Services

It is a general-purpose entry point for keeping an app running in the background
There are two types of services that tell the system how to manage an app:

1. started services
2. bound services.

### Broadcast receivers

It enables the system to deliver events to the app outside of a regular user flow

### Content providers

It manages a shared set of app data that you can store in the file system

## Activating components

Activities, services, and broadcast receivers—are activated by an asynchronous message(intent).

Content providers are activated by a request from a ContentResolver.

## The manifest file

It is the root file of the project, it contains the components of the project.

There are other benefits for the manifest file more than the component definition:

1. Identifies any user permissions the app requires.
2. Declares the minimum API Level required by the app.
3. Declares hardware and software features used or required by the app.
4. Declares API libraries the app needs to be linked.

### Declaring components

We declare all app components using the following elements:

1. `<activity>` elements for activities.
2. `<service>` elements for services.
3. `<receiver>` elements for broadcast receivers.
4. `<provider>` elements for content providers.

### Declaring component capabilities

We use  intent filters to declare the capabilities of the activity.

### Declaring app requirements

It is important to declare app requirements and most of these declarations are informational only and the system does not read them, but external services can read them.

## App resources

* The android app is not a code just it requires resources, such as images, audio files, and anything relating to the visual presentation of the app. and ypu can define these resources using xml files.

* Android supports qualifiers which a short string included in the name of the resource directories in order to define the device configuration.

## Resources used in this reading

1. [Application Fundamentals](https://developer.android.com/guide/components/fundamentals#Components)
