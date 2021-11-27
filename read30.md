# Cognito

Cognito is an AWS product that controls user authentication and access for mobile applications. The service saves and synchronizes end-user data,which make developers focus on the code and that make the development process faster.

* User pools: User directories that provide sign-up and sign-in options for app users.
* Identity pools: Cognito elements grant users access to other AWS services

## Configure Auth Category

1. In the terminal type **amplify add auth**
2. Enter the following when prompted:

   * ? Do you want to use the default authentication and security configuration?
    `Default configuration`
   * ? How do you want users to be able to sign in?
    `Username`
   * ? Do you want to configure advanced settings?
    `No, I am done.`

3. To push your changes to the cloud type **amplify push** in the terminal.

After finishing these steps `amplifyconfiguration.json` should be updated.

## Install Amplify Libraries

to install the auth Amplify libraries we must add **implementation 'com.amplifyframework:aws-auth-cognito:1.30.0'** to the app build.gradle then click sync.

## Initialize Amplify Auth

We must add the Auth plugin before calling `Amplify.configure`.so we add the following lines to the Prerequisites:

```java
// Add this line, to include the Auth plugin.
Amplify.addPlugin(new AWSCognitoAuthPlugin());
Amplify.configure(getApplicationContext());
```

## Check the current auth session

We can check the current auth session by using **Amplify.Auth.fetchAuthSession** from the documentation.

## Resources for this reading

1. [AUTHENTICATION](https://docs.amplify.aws/lib/auth/getting-started/q/platform/android/#check-the-current-auth-session)
