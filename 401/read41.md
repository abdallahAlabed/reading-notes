#  Kinesis & Analytics

Goal
To setup and configure your application with Amplify Analytics and record an analytics event.

Prerequisites
Install and configure Amplify CLI
An Android application targeting Android API level 16 (Android 4.1) or above
For a full example of creating Android project, please follow the project setup walkthrough


Set up Analytics backend
Run the following command in your project's root folder. The CLI will prompt configuration options for the Analytics category such as Amazon Pinpoint resource name and analytics event settings.



amplify add analytics


? Select an Analytics provider (Use arrow keys)
    `Amazon Pinpoint`
? Provide your pinpoint resource name:
    `yourPinpointResourceName`
? Apps need authorization to send analytics events. Do you want to allow guests and unauthenticated users to send analytics events? (we recommend you allow this when getting started)
    `Yes`

    amplify push


    Install Amplify Libraries
Expand Gradle Scripts, open build.gradle (Module: app). You will already have configured Amplify by following the steps in the Project Setup walkthrough.

dependencies {
    // Add these lines in `dependencies`
    implementation 'com.amplifyframework:aws-analytics-pinpoint:1.24.0'
    implementation 'com.amplifyframework:aws-auth-cognito:1.24.0'
}

Click Sync Now

Initialize Amplify Analytics
To initialize the Amplify Auth and Analytics categories you call Amplify.addPlugin() method for each category. To complete initialization call Amplify.configure().

Add the following code to your onCreate() method in your application class:

Amplify.addPlugin(new AWSCognitoAuthPlugin());
Amplify.addPlugin(new AWSPinpointAnalyticsPlugin(this));

Your class will look like this:

public class MyAmplifyApp extends Application {
    @Override
    public void onCreate() {
        super.onCreate();

        try {
            // Add these lines to add the AWSCognitoAuthPlugin and AWSPinpointAnalyticsPlugin plugins
            Amplify.addPlugin(new AWSCognitoAuthPlugin());
            Amplify.addPlugin(new AWSPinpointAnalyticsPlugin(this));
            Amplify.configure(getApplicationContext());

            Log.i("MyAmplifyApp", "Initialized Amplify");
        } catch (AmplifyException error) {
            Log.e("MyAmplifyApp", "Could not initialize Amplify", error);
        }
    }
}


Record events
To record an event, create an AnalyticsEvent and call Amplify.Analytics.recordEvent() to send it:

JavaKotlinRxJava
AnalyticsEvent event = AnalyticsEvent.builder()
    .name("PasswordReset")
    .addProperty("Channel", "SMS")
    .addProperty("Successful", true)
    .addProperty("ProcessDuration", 792)
    .addProperty("UserAge", 120.3)
    .build();

Amplify.Analytics.recordEvent(event);


View Analytics console
From the terminal run the following command.

amplify console analytics
Next Steps:

Congratulations! Now that you have Analytics' backend provisioned and Analytics library installed. Check out the following links to see Amplify Analytics use cases:

Record Events
Track Sessions
Identify User
Escape Hatch

## Sources:
- ### [- Kinesis & Analytics ](https://docs.amplify.aws/lib/analytics/getting-started/q/platform/android/#record-events)