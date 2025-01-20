# Unhandled Exception in Node.js HTTP Server

This repository demonstrates a common yet easily overlooked error in Node.js: unhandled exceptions within an HTTP request handler.  Failure to properly handle exceptions can lead to unexpected crashes and downtime for your server.

## Bug

The `bug.js` file contains a simple HTTP server.  However, if you navigate to `/error`, the server will throw an uncaught exception, causing it to crash.

## Solution

The `bugSolution.js` file shows how to properly handle exceptions using a `try...catch` block, preventing the server from crashing.  The solution also includes improved error logging and sending an appropriate error response to the client.