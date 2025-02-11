# Node.js Server Unresponsiveness

This repository demonstrates a common issue in Node.js servers: unresponsiveness caused by long-running synchronous operations.  The `server.js` file contains a flawed server that performs a 5-second CPU-bound operation, blocking the event loop and preventing it from processing other requests. This leads to the server appearing to hang.

The `serverSolution.js` file provides a corrected version of the server that addresses the issue using asynchronous operations and avoids blocking the event loop.