# Unhandled Error in Express Route Handler: Invalid User ID

This repository demonstrates a common error in Express.js route handlers: failure to handle invalid input, specifically a non-numeric user ID.

The `bug.js` file contains the erroneous code.  It attempts to parse the user ID from the request parameters as an integer without error handling.  If the ID is not a number, the `parseInt` function will return `NaN`, and the subsequent `find` operation might cause unexpected behavior or even a crash.

The `bugSolution.js` file provides a corrected version with robust error handling.