# Unhandled Promise Rejection in Express.js

This repository demonstrates a common error in Node.js applications using Express.js: unhandled promise rejections.  The example code simulates an asynchronous operation that randomly throws an error, leading to the application crashing without proper error handling.  The solution shows how to properly handle this using `try...catch` blocks or promise error handling.

## Bug Description

The `bug.js` file contains an Express.js server with a route that simulates an asynchronous operation.  This operation randomly throws an error, resulting in an unhandled promise rejection, causing the application to terminate abruptly.

## Solution

The `bugSolution.js` file provides a solution by adding proper error handling to catch the exception before it leads to a crash.  It handles potential errors by logging them and returning an error response to the client.