# BroadcastReceiver_examples

**2023-11-13 This repository is archived.**

Android *only* examples of using the Python class `android.broadcast.BroadcastReceiver`.

There are two examples, [WiFi_scanner_example](https://github.com/Android-for-Python/BroadcastReceiver_examples/tree/main/WiFi_scanner_example), and [Bluetooth_scanner_example](https://github.com/Android-for-Python/BroadcastReceiver_examples/tree/main/Bluetooth_scanner_example).

To find a file containing a list of all the Android *system* Broadcast actions for a particular installed `android.api`: on a machine where Buildozer has been run, type `find ~/.buildozer -name broadcast_actions.txt`

**Note:** An instance of `BroadcastReceiver` may only have one call to `start()`. To start a `BroadcastReceiver` again, call `stop()` and create a new instance of `BroadcastReceiver` then call its `start()`.
