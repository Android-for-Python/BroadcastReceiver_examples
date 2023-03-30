# Bluetooth_scanner_example

Android *only* example of using the Python class `android.broadcast.BroadcastReceiver`.

This example does *not* require that Android location services are enabled.

If you wish to extend the example in a way that uses location services:

1) in `buildozer.spec` replace:

```
android.permissions = (name=android.permission.BLUETOOTH_SCAN;usesPermissionFlags=neverForLocation)
```
with:
```
android.permissions = BLUETOOTH_SCAN, ACCESS_FINE_LOCATION
```

2)  in `android_permissions.py` replace:

```python
            self.permissions = [Permission.BLUETOOTH_SCAN]
```
with:
```python
            self.permissions = [Permission.BLUETOOTH_SCAN,
                                Permission.ACCESS_FINE_LOCATION]
```

