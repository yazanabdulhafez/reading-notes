# Notifications

## What is Amazon SNS?

Amazon Simple Notification Service (Amazon SNS) it is a service allow the owner of the application to communicate asynchronously with the people who use the application by sending a notifications.

Amazon SNS push notifications aren't available in all AWS Regions.

To use this service we must do the following:

## Add The project to Firebase

1. Create a Firebase project and register your app
2. Install the SDK and initialize Firebase
3. Access Firebase in your app
4. Use a module bundler (webpack/Rollup) for size reduction

### create project in Firebase

1. In the Firebase console, click Add project.
2. If prompted, review and accept the Firebase terms.
3. Click Continue.
4. Add Firebase

### Register your app with Firebase

1. Go to the Firebase console.

2. In the center of the project overview page, click the Android icon (plat_android) or Add app to launch the setup workflow.

3. Enter your app's package name in the Android package name field.

4. (Optional) Enter other app information

5. Click Register app.

### Add a Firebase configuration file

1. Add the Firebase Android configuration file to your app:

   * Click Download google-services.json to obtain your Firebase Android config file (google-services.json).

   * Move your config file into the module (app-level) directory of your app.

2. To enable Firebase products in your app, add the google-services plugin to your Gradle files.

### Add Firebase SDKs to your app

1. Using the Firebase Android BoM, declare the dependencies for the Firebase products.

2. Sync the app

## Copy your FCM project's API key

1. In the Firebase console, choose your project.

2. In the left navigation pane, choose the gear icon, and then choose Project settings.

3. Choose Cloud Messaging.

4. Under Project credentials, find the Server key. This your FCM project's API key. Copy it to your clipboard.

## Create a platform application in Amazon SNS

1. Open the Amazon SNS console.

2. In the left navigation pane, choose Mobile. Then, choose Push notifications.

3. On the Mobile push notifications page, next to Platform applications, choose Create platform application.

4. On the Create platform application page, under Details, do the following:

   * For Application name, enter the name of your application.
   * For Push notification platform, choose Firebase Cloud Messaging (FCM).
   * Under Firebase Cloud Messaging Credentials, for API key, enter the server key that you copied earlier.

5. (Optional) Set up event notifications and delivery status logging.

6. Choose Create platform application.

## SNS Benefits and features

1. Reliably deliver messages with durability
2. Automatically scale your workload
3. Simplify your architecture with Message Filtering
4. Keep messages private and secure

## Resources used in this reading

1. [Create project on Firebase](https://firebase.google.com/docs/android/setup)

2. [create an Android platform application in Amazon SNS](https://aws.amazon.com/ar/premiumsupport/knowledge-center/create-android-push-messaging-sns/)

3. [Amazon Simple Notification Service](https://console.aws.amazon.com/sns/v3/home?region=us-east-1#/homepage)
