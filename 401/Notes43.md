# Read: Class 43 Read: 43 - Kinesis & Analytics

## [Amplify and Kinesis](https://docs.amplify.aws/lib/analytics/getting-started/q/platform/android/)

### Set up Analytics backend

1. Run the following command in your project's root folder. The CLI will prompt configuration options for the Analytics category such as Amazon Pinpoint resource name and analytics event settings.
   `amplify add analytics`
1. Upon completion, amplifyconfiguration.json should be updated to reference provisioned backend analytics resources.

### Install Amplify Libraries

### Initialize Amplify Analytics

To initialize the Amplify Auth and Analytics categories you call Amplify.addPlugin() method for each category. To complete initialization call Amplify.configure().

### Record events

To record an event, create an AnalyticsEvent and call Amplify.Analytics.recordEvent() to send it:

```java
AnalyticsEvent event = AnalyticsEvent.builder()
    .name("PasswordReset")
    .addProperty("Channel", "SMS")
    .addProperty("Successful", true)
    .addProperty("ProcessDuration", 792)
    .addProperty("UserAge", 120.3)
    .build();

Amplify.Analytics.recordEvent(event);
```