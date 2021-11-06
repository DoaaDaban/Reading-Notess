# Espresso

Espresso is an open source android user interface (UI) testing framework.

Espresso’s API Components:

1. **Espresso**: This is the starting point for all test cases. This component provides entry points or methods to start the interaction with the app’s view. Each app’s view has two components.

2. **ViewMatchers**: Views are always in a hierarchy called the View Hierarchy. For the test cases to navigate the view hierarchy, ViewMatchers are used.

3. **ViewActions**: These components define the action that has to be performed on any given View. Espresso allows testers to send more than one ViewAction as a collection to the Interaction method.

4. **ViewAssertions**: They are the components that check if the test has passed or failed. 

## fnctions:

1. **onView**: Using this function, we can narrow down to the desired view in the view hierarchy. It can be done by using the following functions inside `onview`:
   
   * `withId()`: With this function, we can narrow down the view search using ids of the view.

   * `withText()`: Here we can pass the desired text to narrow down the views based on the text.

2. **check**: This is used to check the behavior of the desired view, like visibility, focus, and more using `matches` and `doesNotExist`.

3. **perform**: Through `perform`, we can execute actions on the views. Following are some of the actions that we can execute using Espresso:

    * `click()`:  Clicks the view passed in `onView`.

    * `typeText()`: Through this function, we can pass the string to be entered in the view. This comes handy with `EditText`.

    * `replaceText()`: Replaces the current text with the string that’s passed.

    * `closeSoftKeyboard()`: Dismisses the keyboard.