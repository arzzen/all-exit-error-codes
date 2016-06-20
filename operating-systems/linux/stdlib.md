# Stdlib Exit Codes 

This list is heavily based on  

* http://tldp.org/LDP/abs/html/exitcodes.html 
* http://stackoverflow.com/questions/1101957/are-there-any-standard-exit-status-codes-in-linux
* http://pocoproject.org/docs/Poco.Util.Application.html#16218


**stdlib.h**

    #define EXIT_FAILURE    1       
    #define EXIT_SUCCESS    0
    The 11 on segfault is interesting, as 11 is the signal number that the kernel uses to kill the process in the event of a segfault.
  


