# Play Services Error Codes

This list is heavily based on

* https://developers.google.com/android/reference/com/google/android/gms/common/ConnectionResult#top_of_page

**Connection failure error Codes**

    API_UNAVAILABLE = 16, /*One of the API components you attempted to connect to is not available*/
    CANCELED = 13, /*The connection was canceled*/
    DEVELOPER_ERROR = 10, /*The application is misconfigured*/
    DRIVE_EXTERNAL_STORAGE_REQUIRED = 1500, /*DEPRECATED*/
    INTERNAL_ERROR = 8, /*An internal error occurred*/
    INTERRUPTED	= 15, /*An interrupt occurred while waiting for the connection complete*/
    INVALID_ACCOUNT = 5, /*The client attempted to connect to the service with an invalid account name specified*/
    LICENSE_CHECK_FAILED = 11, /*The application is not licensed to the user*/
    NETWORK_ERROR = 7, /*A network error occurred*/
    RESOLUTION_REQUIRED = 6, /*Completing the connection requires some form of resolution*/
    RESTRICTED_PROFILE = 20, /*The current user profile is restricted and cannot use authenticated features*/
    SERVICE_DISABLED = 3, /*The installed version of Google Play services has been disabled on this device*/
    SERVICE_INVALID = 9, /*The version of the Google Play services installed on this device is not authentic*/
    SERVICE_MISSING = 1, /*Google Play services is missing on this device*/
    SERVICE_MISSING_PERMISSION = 19, /*Google Play service doesn't have one or more required permissions*/
    SERVICE_UPDATING = 18, /*Google Play service is currently being updated on this device*/
    SERVICE_VERSION_UPDATE_REQUIRED = 2, /*The installed version of Google Play services is out of date*/
    SIGN_IN_FAILED = 17, /*The client attempted to connect to the service but the user is not signed in*/
    SIGN_IN_REQUIRED = 4, /*The client attempted to connect to the service but the user is not signed in*/
    SUCCESS = 0, /*The connection was successful*/
    TIMEOUT = 14, /*The timeout was exceeded while waiting for the connection to complete*/
    ERROR_MAX_CAMERAS_IN_USE = 2, /*Camera device could not be opened because there are too many other open camera devices*/
