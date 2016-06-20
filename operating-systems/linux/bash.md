# Bash Exit Codes 

This list is heavily based on  

* http://tldp.org/LDP/abs/html/exitcodes.html 
* http://stackoverflow.com/questions/1101957/are-there-any-standard-exit-status-codes-in-linux

**Advanced Bash-Scripting**

    1: Catchall for general errors
    2: Misuse of shell builtins (according to Bash documentation)
    126: Command invoked cannot execute
    127: "command not found"
    128: Invalid argument to exit
    128+n: Fatal error signal "n"
    130: Script terminated by Control-C 
    255: Exit status out of range (exit takes only integer args in the range 0 - 255)
