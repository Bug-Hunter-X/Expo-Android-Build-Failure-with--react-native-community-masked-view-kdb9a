# Expo Android Build Failure with @react-native-community/masked-view

This repository demonstrates a bug encountered when building an Android app using Expo CLI and the `@react-native-community/masked-view` package. The build process fails with ambiguous error messages, making debugging challenging.

## Bug Description
The core issue is that the Android build system fails during the build process, frequently without clear error details related to `masked-view`.  This leads to significant time loss in debugging.  The bug often manifests after seemingly successful installation and linking of the package.

## Steps to Reproduce
1.  Create a new Expo project: `expo init my-app`
2.  Install the package: `expo install @react-native-community/masked-view`
3.  Attempt to build the Android app: `expo build:android`

## Solution
The solution involves a combination of steps aiming to clean up the Android build system, ensuring proper linking, and verifying dependencies. The details are included in the `bugSolution.js` file and demonstrate the successful build process.