#Perl Error Variables

This list comes from [Perldoc Website](https://perldoc.perl.org/perlvar.html#Error-Variables).
I encourage you to read detailed informations about those variables from Perldoc.

| Error Variable  | Error English Name    | Description  |
| :-------------: |:-------------| ------------|
| $@ | $EVAL_ERROR | The Perl error from the last eval operator, i.e. the last exception that was caught.|
| $! | $ERRNO and $OS_ERROR | When referenced, $! retrieves the current value of the C errno integer variable. [See Also: ](https://github.com/arzzen/all-exit-error-codes/blob/master/programming-languages/c/errors.md) |
| $^E | $EXTENDED_OS_ERROR | Error information specific to the current operating system.|
| $? | $CHILD_ERROR | Status from the las wait() call.|
|    | ${CHILD_ERROR_NATIVE} | The native status returned by the last child process (v5.10+).|
