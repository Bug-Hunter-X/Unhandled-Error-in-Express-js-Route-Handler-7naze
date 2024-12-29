# Unhandled Error in Express.js Route Handler

This repository demonstrates a common error in Express.js route handlers:  missing error handling for invalid input.  The `bug.js` file shows the problematic code, while `bugSolution.js` provides a corrected version.

The bug occurs when the route `/users/:id` receives an invalid `id` parameter. The code attempts to parse the ID as an integer and search for a matching user.  However, no error handling is present if the ID is not a valid integer, resulting in an unhandled exception.

The solution adds robust error handling to check for both non-numeric and non-existent user IDs, returning appropriate HTTP error codes and messages.