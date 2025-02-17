# Node.js Server Hanging Issue

This repository demonstrates a common issue in Node.js where long-running requests can cause the server to hang, becoming unresponsive to other requests.  The provided code simulates a long-running operation, which blocks the event loop and prevents the server from processing other requests.

## Bug Description

The `server.js` file contains a simple HTTP server.  However, it includes a `while` loop that simulates a 5-second delay.  During this delay, the server is unable to handle any additional requests, leading to a unresponsive server and a poor user experience.

## Solution

The `serverSolution.js` file provides a solution to this problem using asynchronous operations and proper handling of requests.  This prevents blocking the event loop and ensures the server remains responsive to other requests.  The solution utilizes asynchronous programming to avoid blocking the event loop.