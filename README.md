# Uncommon Expo CLI Crash/Hang During Build and Start

This repository demonstrates an uncommon bug encountered with the Expo CLI resulting in unexpected crashes or hangs during development.  The issue is particularly challenging to diagnose due to its inconsistent nature. This example shows a potential scenario and provides a suggested solution.

## Bug Description

The bug causes the Expo CLI to crash or hang during various commands (e.g., `expo start`, `expo build:ios`, `expo publish`). The error messages are inconsistent but often hint at problems with native module compilation or interactions within Expo Go. This is especially likely in complex projects with multiple dependencies and custom native modules.

## Reproduction Steps

1. Clone this repository
2. Run `npm install` or `yarn install`
3. Attempt to run `expo start`
4. (Potentially) Observe crash or hang

## Solution

See `expoBugSolution.js` for a potential fix. This may involve clearing the cache, upgrading dependencies, or investigating potential conflicts between native modules.