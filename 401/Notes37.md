# Amazon S3

## Introduction to Amazon S3

Amazon Simple Storage Service (Amazon S3) is a scalable, high-speed, web-based cloud storage service. The service is designed for online backup and archiving of data and applications on Amazon Web Services.

### Advantages of using Amazon S3

1. Creating buckets: Create and name a bucket that stores data. Buckets are the fundamental containers in Amazon S3 for data storage.

2. Storing data: Store an infinite amount of data in a bucket.

3. Downloading data: Download your data or enable others to do so. Download your data anytime you like, or allow others to do the same.

4. Permissions: Grant or deny access to others who want to upload or download data into your Amazon S3 bucket.

5. Standard interfaces: Use standards-based REST and SOAP interfaces designed to work with any internet-development toolkit.

### Amazon S3 concepts

1. **Buckets**: A bucket is a container for objects stored in Amazon S3. Every object is contained in a bucket and its Names must be unique.

2. **Objec**: Objects are the fundamental entities stored in Amazon S3. Objects consist of object data and metadata. The data portion is opaque to Amazon S3. The metadata is a set of name-value pairs that describe the object.

3. **Keys**: A key is the unique identifier for an object within a bucket. Every object in a bucket has exactly one key.

4. **Regions**: ou can choose the geographical AWS Region where Amazon S3 will store the buckets that you create.

## S3 with Amplify

1. To start provisioning storage resources in the backend, go to your project directory and execute the command: `amplify add storage`.

2. Enter the following when prompted:

```
? Please select from one of the below mentioned services:
    `Content (Images, audio, video, etc.)`
? You need to add auth (Amazon Cognito) to your project in order to add storage for user files. Do you want to add auth now?
    `Yes`
? Do you want to use the default authentication and security configuration?
    `Default configuration`
? How do you want users to be able to sign in?
    `Username`
? Do you want to configure advanced settings?
    `No, I am done.`
? Please provide a friendly name for your resource that will be used to label this category in the project:
    `S3friendlyName`
? Please provide bucket name:
    `storagebucketname`
? Who should have access:
    `Auth and guest users`
? What kind of access do you want for Authenticated users?
    `create/update, read, delete`
? What kind of access do you want for Guest users?
    `create/update, read, delete`
? Do you want to add a Lambda Trigger for your S3 Bucket?
    `No`
```

3. push your changes to the cloud, execute the command: `amplify push`.

4. Install amplify libraries by adding these libraries into the dependencies block:

```
dependencies {
    implementation 'com.amplifyframework:aws-storage-s3:1.24.0'
    implementation 'com.amplifyframework:aws-auth-cognito:1.24.0'
}
```