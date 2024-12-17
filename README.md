# Tailwind CSS PurgeCSS Error

This repository demonstrates a common error encountered when using Tailwind CSS's PurgeCSS feature.  The error occurs when a class used in your application is inadvertently removed during the build process, leading to a runtime `ReferenceError`. This example shows how to fix this issue by ensuring that the classes remain in the output CSS.

## Steps to reproduce

1. Clone this repository.
2. Run `npm install` to install the dependencies.
3. Run `npm run build` to build the application and observe the error.
4. Open the `bugSolution.js` file to see the corrected version.

## How to fix

The problem occurs because the `bg-red-500` class was removed during the purge process. The fix involves ensuring that the class is correctly included in your Tailwind configuration or explicitly whitelisted. The corrected code includes it in your configuration.