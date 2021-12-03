# Intent Filters

* An Intent filter is used to allow other applications to start activity that contain it. and to do this we need to add an `<intent-filter>` element in  manifest file for the corresponding `<activity>` element.

* The system identifies the intent filters when the application installed on the device and When an app calls startActivity() or startActivityForResult(), with an implicit intent, the system finds which activity (or activities) can respond to the intent.

## Add an Intent Filter

Criteria of the Intent object:

1. Action: A string naming the action to perform
2. Data:it is a description of the data associated with the intent
3. Category: it Provides an additional way to characterize the activity handling the intent

when intent filter fulfil these criterions we can add it in the manifest file.

## Handle the Intent in Your Activity

* At the start of our activity, we call getIntent() to retrieve the Intent that started the activity. this can be done at any time in cycle life, but preferred doing this at early callbacks such as onCreate() or onStart().

## Return a Result

* If we want to return a result to the activity that invoked our application, simply call setResult() and When our operation is done call finish() to destroy our activity.

## Resources used in this reading

1. [Allowing Other Apps to Start Your Activity](https://developer.android.com/training/basics/intents/filters)
2. [Android Intent Filters](https://docs.axway.com/bundle/Titanium_SDK_allOS_en/page/android_intent_filters.html)
