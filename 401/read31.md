# Espresso

## Create UI tests with Espresso Test Recorder
### The Espresso Test Recorder tool lets you create UI tests for your app without writing any test code. By recording a test scenario, you can record your interactions with a device and add assertions to verify UI elements in particular snapshots of your app. 
## Record an Espresso test
### * Click Run > Record Espresso Test.
### * In the Select Deployment Target window, choose the device on which you want to record the test
### * Espresso Test Recorder triggers a build of your project, and the app must install and launch before Espresso Test Recorder allows you to interact with it. The Record Your Test window appears after the app launches, and since you have not interacted with the device yet, the main panel reads "No events recorded yet." Interact with your device to start logging events such as "tap" and "type" actions.
## Save a recording
## Run an Espresso test with Firebase Test Lab for Android

## Target audience
### Espresso is targeted at developers, who believe that automated testing is an integral part of the development lifecycle. While it can be used for black-box testing, Espresso’s full power is unlocked by those who are familiar with the codebase under test.

## Synchronization capabilities
### Each time your test invokes onView(), Espresso waits to perform the corresponding UI action or assertion until the following synchronization conditions are met:

### * The message queue is empty.
### * There are no instances of AsyncTask currently executing a task.
### * All developer-defined idling resources are idle.
### By performing these checks, Espresso substantially increases the likelihood that only one UI action or assertion can occur at any given time. This capability gives you more reliable and dependable test results
## Sources:



- ### [- Espresso Testing (read Overview, Basics, and Recipes, plus any others that look interesting)](https://developer.android.com/training/testing/espresso)
- ### [- Ridiculous superpower: the Espresso Test Recorder](https://developer.android.com/studio/test/espresso-test-recorder)