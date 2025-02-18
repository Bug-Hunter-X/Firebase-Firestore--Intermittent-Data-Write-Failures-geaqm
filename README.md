# Firebase Firestore Intermittent Write Failure

This repository demonstrates a bug encountered with Firebase Firestore where data writes fail intermittently without any apparent errors in the console. The issue is particularly challenging to debug as it is not consistent and doesn't provide clear error messages.

The `firestoreBug.js` file contains code that attempts to write data to Firestore.  The `firestoreBugSolution.js` file offers a solution for handling potential write failures.

## Reproducing the Bug

Follow these steps to try and reproduce the bug:
1.  Clone this repository.
2.  Set up a Firebase project and install the necessary dependencies.
3.  Run the `firestoreBug.js` file.
4.  Observe the Firestore database. Note that data may or may not be written successfully.  Inconsistent behavior is the key indicator of this bug.

## Solution

The `firestoreBugSolution.js` file incorporates error handling and retry mechanisms to address the intermittent write failure.