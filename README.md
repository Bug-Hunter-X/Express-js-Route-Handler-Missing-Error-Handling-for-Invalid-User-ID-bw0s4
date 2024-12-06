# Express.js Route Handler Missing Error Handling for Invalid User ID

This repository demonstrates a common error in Express.js route handlers: the lack of proper error handling for invalid input.  Specifically, this example shows a route that fetches a user by ID but fails to handle cases where the ID is not a valid number. This can lead to unexpected behavior or even crashes.

## The Bug

The `bug.js` file contains an Express.js route handler that fetches a user by ID. However, it does not handle cases where the `userId` parameter is not a valid number. This can result in an error if a user tries to access a route with an invalid ID.

## The Solution

The `bugSolution.js` file provides a corrected version of the route handler. This version includes error handling to gracefully handle cases where the `userId` parameter is not a valid number.  The solution includes checks to ensure the ID is a number and returns appropriate error responses if it isn't.