# React Router Dom Wildcard Route (*) Unexpected Behavior

This repository demonstrates an uncommon bug in React Router Dom v6 where the wildcard route (`*`) does not always catch all unmatched paths as expected.  The issue is particularly evident when dealing with dynamic segments or nested routes that result in invalid or unexpected route matching behavior.

## Bug Description

The provided `App.js` demonstrates a seemingly straightforward React Router setup.  However, under certain conditions (e.g., manual URL manipulation, invalid paths), the wildcard route fails to render the 404 component, leading to unexpected behavior.

## Solution

The `AppSolution.js` illustrates a corrected implementation with changes that ensures the `*` route works consistently across different scenarios. Key considerations for resolving this include careful handling of route matching prioritization and potential edge cases related to dynamic segment matching. 