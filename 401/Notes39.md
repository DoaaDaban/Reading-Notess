# Amplify and Kinesis

* The Analytics category enables you to collect analytics data for your App.

* Amazon Kinesis makes it easy to collect, process, and analyze real-time, streaming data so you can get timely insights and react quickly to new information.

## Benefits

1. **Real-time**: Amazon Kinesis enables you to ingest, buffer, and process streaming data in real-time, so you can derive insights in seconds or minutes instead of hours or days.

2. **Fully managed**: Amazon Kinesis is fully managed and runs your streaming applications without requiring you to manage any infrastructure.

3. **Scalable**: Amazon Kinesis can handle any amount of streaming data and process data from hundreds of thousands of sources with very low latencies.

## Set up Analytics backend:

Run the following command in your project’s root folder:

1. `amplify add analytics`

2. Enter the following when prompted:

```
? Select an Analytics provider (Use arrow keys)
    `Amazon Pinpoint`
? Provide your pinpoint resource name:
    `yourPinpointResourceName`
? Apps need authorization to send analytics events. Do you want to allow guests and unauthenticated users to send analytics events? (we recommend you allow this when getting started)
    `Yes`
```

3. push your changes to the cloud, execute the command: `amplify push`.

4. Install Amplify Libraries by adding these libraries into the dependencies block:

```
dependencies {
    // Add these lines in `dependencies`
    implementation 'com.amplifyframework:aws-analytics-pinpoint:1.24.0'
    implementation 'com.amplifyframework:aws-auth-cognito:1.24.0'
}
```