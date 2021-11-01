#  Intents, Activities, and SharedPreferences

## Android Tasks and the Back Stack

* A task is a collection of activities that users interact with when performing a certain job. These activities are arranged in the order in the stack.

* When the user selects a new activity that means this new activity will add to the top of the stack.

* Home screen is the starting place for most tasks.

* When the user presses the **Back** button that means the new activity is finished and popped off from the top of the stack.

### Managing Tasks

The attributes in the `<activity>` manifest element is used to managing tasks. The pruncipal `<activity>` attributes we can use are:

* `taskAffinity`

* `launchMode`

* `allowTaskReparenting`

* `clearTaskOnLaunch`

* `alwaysRetainTaskState`

* `finishOnTaskLaunch`

## Android SharedPreferences

* **Save key-value data**: A `SharedPreferences` APIs is used to save a relatively small collection of key-values

* **Get a handle to shared preferences**: 

    * `getSharedPreferences()`: Use this if you need multiple shared preference files identified by name, which you specify with the first parameter.

    * `getPreferences()`: Use this from an Activity if you need to use only one shared preference file for the activity.