# Cognito

Amazon Cognito is a robust user directory service that handles user registration, authentication, account recovery & other operations.

## Configure Auth Category:

1. To start provisioning auth resources in the backend, go to your project directory and execute the command `amplify add auth`.

2. Enter the following when prompted:

```
? Do you want to use the default authentication and security configuration?
    `Default configuration`
? How do you want users to be able to sign in?
    `Username`
? Do you want to configure advanced settings?
    `No, I am done.`
```

3. Last step in terminal is push the changes by `amplify push` command.

4. Now add the following dependency to your app’s **build.gradle**:

```
dependencies {
implementation ‘com.amplifyframework:aws-auth-cognito:1.24.0’
}
```

## Advantages of AWS Cognito:

1. Consistent Experience Across Multiple Devices

Cognito is built to handle multi-device authentication seamlessly, enabling your users to use the same login on their web, mobile and desktop applications.

2. Guest Logins

Another useful feature of Cognito is its ability to allow guest logins to your product

3. Social Media Logins

Cognito allows integration with third-party authentication systems like Google and Facebook, thereby providing more options for your users while signing up for your product.