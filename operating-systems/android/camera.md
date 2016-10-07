# Camera Error Codes

This list is heavily based on

* https://developer.android.com/reference/android/hardware/camera2/CameraDevice.StateCallback.html

**Camera error Codes**

    ERROR_CAMERA_DEVICE = 4, /*Camera device has encountered a fatal error*/  	
    ERROR_CAMERA_DISABLED = 3, /*Camera device could not be opened due to a device policy*/
    ERROR_CAMERA_IN_USE = 1, /*Camera device is in use already*/
    ERROR_CAMERA_SERVICE = 5, /*Camera service has encountered a fatal error*/
    ERROR_MAX_CAMERAS_IN_USE = 2, /*Camera device could not be opened because there are too many other open camera devices*/
