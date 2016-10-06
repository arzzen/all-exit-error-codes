# Twitter API Error Codes

This list comes directly from [Twitter's Pulic API response codes page](https://dev.twitter.com/overview/api/response-codes).

#### HTTP Status Codes
The Twitter API attempts to return appropriate HTTP status codes for every request

| HTTP Error Code  | Text    | Description  |
| :-------------: |:-------------| ------------|
| 200 | OK | Node.js will normally exit with a 0 status code when no more async operations are pending.|
| 304 | Uncaught Fatal Exception | There was an uncaught exception, and it was not handled by a domain or an 'uncaughtException' event handler.  |
| 400 | N/A | Reserved by Bash for builtin misuse |
| 401 | Internal JavaScript Parse Error | The JavaScript source code internal in Node.js's bootstrapping process caused a parse error. This is extremely rare, and generally can only happen during development of Node.js itself. |
| 403 | Internal JavaScript Evaluation Failure | The JavaScript source code internal in Node.js's bootstrapping process failed to return a function value when evaluated. This is extremely rare, and generally can only happen during development of Node.js itself. |
| 404 | Fatal Error | There was a fatal unrecoverable error in V8. Typically a message will be printed to stderr with the prefix FATAL ERROR. |
| 406 | Non-function Internal Exception Handler | There was an uncaught exception, but the internal fatal exception handler function was somehow set to a non-function, and could not be called. |
| 410 | Internal Exception Handler Run-Time Failure | There was an uncaught exception, and the internal fatal exception handler function itself threw an error while attempting to handle it. This can happen, for example, if a 'uncaughtException' or domain.on('error') handler throws an error. |
| 420 | N/A | In previous versions of Node.js, exit code 8 sometimes indicated an uncaught exception. |
| 422 | Invalid Argument | Either an unknown option was specified, or an option requiring a value was provided without a value. |
| 429 | Internal JavaScript Run-Time Failure | The JavaScript source code internal in Node.js's bootstrapping process threw an error when the bootstrapping function was called. This is extremely rare, and generally can only happen during development of Node.js itself. |
| 500 | Internal Server Error | The --debug, --inspect and/or --debug-brk options were set, but the port number chosen was invalid or unavailable. |
| 502 | Bad Gateway	 | If Node.js receives a fatal signal such as SIGKILL or SIGHUP, then its exit code will be 128 plus the value of the signal code. This is a standard Unix practice, since exit codes are defined to be 7-bit integers, and signal exits set the high-order bit, and then contain the value of the signal code. |
| 503 | Service Unavailable | If Node.js receives a fatal signal such as SIGKILL or SIGHUP, then its exit code will be 128 plus the value of the signal code. This is a standard Unix practice, since exit codes are defined to be 7-bit integers, and signal exits set the high-order bit, and then contain the value of the signal code. |
| 504 | Gateway timeout | If Node.js receives a fatal signal such as SIGKILL or SIGHUP, then its exit code will be 128 plus the value of the signal code. This is a standard Unix practice, since exit codes are defined to be 7-bit integers, and signal exits set the high-order bit, and then contain the value of the signal code. |
