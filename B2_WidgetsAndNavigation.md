# Widgets and navigation

You will need to read about different widgets and UI navigation elements available in the platform.

There are tons of other widgets than the ones you will encounter that can be used in your projects, you can browse them [here](https://developer.android.com/reference/android/widget/package-summary.html). You don't need to know them well, just to know that such widgets exist. You can dig deeper when you need to use them.

Sometimes a widget that you need is not available in the platform. In this case usually you can find some open source library in github that implements such a widget which you can then import it in your project. Aim for ones with higher number of stars. In some cases there are no such libraries and we need to write our own custom views. We'll do this in some of the next projects.

Your task is to create an app with several screens (activities).

## Main screen
Here you have a choice of 2 screens: "Screen 1", "Screen 2" as [buttons](https://developer.android.com/guide/topics/ui/controls/button.html). Clicking on each button opens a new screen. For opening a different activity you need to know about [intents](https://developer.android.com/guide/components/intents-filters.html).

## Screen 1
Here you have an [EditText](https://developer.android.com/reference/android/widget/EditText.html) where you can input some text. There are three buttons - the first one opens a [toast](https://developer.android.com/guide/topics/ui/notifiers/toasts.html) with the string from the EditText, the second one opens a [snackbar](https://developer.android.com/training/snackbar/index.html) with the string (with a single button which closes the snackbar) and the third one opens a [dialog](https://developer.android.com/guide/topics/ui/dialogs.html) which also shows the string. [Back button](https://developer.android.com/reference/android/app/Activity.html#onBackPressed()) action should clear the string in the EditText and if the text is empty should close the current activity.

## Screen 2
Here you have a [spinner](https://developer.android.com/guide/topics/ui/controls/spinner.html) (a form of dropdown selection menu) with different options (random strings). Automatically display the selected option in a [TextView](https://developer.android.com/reference/android/widget/TextView.html). Also you should have (at least) 3 [radio buttons](https://developer.android.com/guide/topics/ui/controls/radiobutton.html) with options such as "Bold", "Italic", "Normal"... Find different variants for formatting the text in a TextView. Depending on the selected option the string selected from the spinner will be using this formatting in the TextView.