# Expo CLI Development Server Random Crashes

This repository demonstrates a bug encountered with the Expo CLI development server where the server crashes randomly without providing any meaningful error messages. The app continues to function on the device/simulator, but live reload ceases to work. This issue is intermittent and occurs without a clear pattern or trigger.

## Steps to Reproduce

1. Clone this repository.
2. Run `npm install`.
3. Run `expo start`.
4. Observe the development server for random crashes.  These crashes will manifest as the server seemingly hanging, with no new terminal output upon making code changes.  The app itself will continue running.

## Potential Solutions

The provided `expoBugSolution.js` offers a suggested solution which involves checking for memory leaks, ensuring proper cleanup of resources, and using more robust error handling.