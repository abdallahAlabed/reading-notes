# Intent Filters
## Allowing Other Apps to Start Your Activity
#### To allow other apps to start your activity by performing an action that might be useful from this app, you need to add an <intent-filter> element in your manifest file for the corresponding <activity> element.

#### the system identifies your intent filters and adds the information to an internal catalog of intents supported by all installed apps. When an app calls startActivity() or startActivityForResult(), with an implicit intent, the system finds which activity (or activities) can respond to the intent.

### Add an Intent Filter
#### The system may send a given Intent to an activity if that activity has an intent filter fulfills the following criteria of the Intent object.

### [Action]

#### Specify this in your intent filter with the <action> element. The value you specify in this element must be the full string name for the action, instead of the API constant.

### [Data]

#### A description of the data associated with the intent. Specify this in your intent filter with the <data>element. Using one or more attributes in this element, indicate the data type accepted.

### [Category]

#### Provides an additional way to characterize the activity handling the intent, usually related to the user gesture or location from which it’s started.

## Sources:
- ### [- Intent Filters ](https://developer.android.com/training/basics/intents/filters)