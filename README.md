# Unhandled Exception in Asynchronous Express.js Route

This repository demonstrates a common error in Node.js Express.js applications: unhandled exceptions within asynchronous route handlers.  When an error occurs within a `setTimeout`, `setInterval`, or other asynchronous operation, it can easily go uncaught, leading to application crashes.

The `bug.js` file contains the problematic code. The `bugSolution.js` provides a corrected version that properly handles the error using `try...catch` blocks.

## How to Reproduce

1. Clone this repository.
2. Navigate to the directory.
3. Run `node bug.js`.
4. Observe that the server will often crash after a short time.  Refresh the browser to see the error.
5. Then Run `node bugSolution.js` and notice the more robust error handling.