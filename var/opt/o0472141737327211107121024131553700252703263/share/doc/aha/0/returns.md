Returns
=======

Most internal functions follow the convention that a return of `0` indicates no error,
while a nonzero return indicates an error.
Rarely, the type of error may be indicated by the value of the return.

A few functions do not return.
These typically call for `exit`ing the program if they fail.
