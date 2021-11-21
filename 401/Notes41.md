# Intent Filters

The intent is a messaging object which tells what kind of action to be performed. The intent’s most significant use is the launching of the activity. Intent facilitates the communication between the components.

Use case of Intents:

1. Starting Activity.

2. Starting a Service.

3. Delivering a Broadcast.

## Intent Type:

1. **Explicit intent**: Explicit intent can do the specific application action which is set by the code like changing activity, In explicit intent user knows about all the things like after clicking a button which activity will start and Explicit intents are used for communication inside the application.

2. **Implicit Intent**: Implicit intents do not name a specific component like explicit intent, instead declare general action to perform, which allows a component from another app to handle.

## Add an Intent Filter

In order to properly define which intents your activity can handle, each intent filter you add should be as specific as possible in terms of the type of action and data the activity accepts.

The system may send a given Intent to an activity if that activity has an intent filter fulfills the following criteria of the `Intent` object:

1. **Action**:  A string naming the action to perform. Usually one of the platform-defined values such as ACTION_SEND or ACTION_VIEW.

2. **Data**: `<data>` A description of the data associated with the intent.

3. **Category**: `<category>` Provides an additional way to characterize the activity handling the intent.

* Each incoming intent specifies only one action and one data type, but it’s OK to declare multiple instances of the `<action>`, `<category>`, and `<data>` elements in each `<intent-filter>`.

* If any two pairs of action and data are mutually exclusive in their behaviors, you should create separate intent filters to specify which actions are acceptable when paired with which data types.