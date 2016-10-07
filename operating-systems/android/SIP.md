# SIP Error Codes

This list is heavily based on  

* https://developer.android.com/reference/android/net/sip/SipErrorCode.html

**SIP errors**

    CLIENT_ERROR = -4, /*When some error occurs on the device, possibly due to a bug*/
    CROSS_DOMAIN_AUTHENTICATION = -11, /*Cross-domain authentication required*/
    DATA_CONNECTION_LOST = -10, /*When data connection is lost*/
    INVALID_CREDENTIALS = -8, /*When invalid credentials are provided*/
    IN_PROGRESS = -9, /*The client is in a transaction and cannot initiate a new one*/
    NO_ERROR = 0, /*Not an error*/
    PEER_NOT_REACHABLE = -7, /*When the peer is not reachable*/
    SERVER_ERROR = -2, /*When server responds with an error*/
    SERVER_UNREACHABLE = -12, /*When the server is not reachable*/
    SOCKET_ERROR = -1, /*When some socket error occurs*/
    TIME_OUT = -5, /*When the transaction gets timed out*/
    TRANSACTION_TERMINTED = -3, /*When transaction is terminated unexpectedly*/
