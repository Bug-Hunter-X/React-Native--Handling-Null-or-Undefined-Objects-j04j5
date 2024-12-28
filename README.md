# React Native: Handling Null or Undefined Objects

This repository demonstrates a common error in React Native applications: attempting to access properties of null or undefined objects.  The `bug.js` file showcases the problematic code, which throws a `TypeError: Cannot read properties of null (reading 'name')` when the fetched data is initially null.  The `bugSolution.js` file provides a solution to safely handle this scenario, preventing the error.

## How to reproduce the bug

1. Clone this repository.
2. Run `npm install` to install dependencies.
3. Run `npx react-native run-android` (or `npx react-native run-ios`) to start the application.
4. Observe the error in the console.

## Solution

The solution involves using optional chaining (`?.`) and nullish coalescing (`??`) operators to safely access the property, or providing a default value.