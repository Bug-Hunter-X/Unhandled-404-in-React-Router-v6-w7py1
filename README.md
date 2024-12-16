# React Router v6 - Missing 404 Route

This repository demonstrates a common error in React Router v6: failing to include a route to handle 404 (Not Found) errors.  Without a catch-all route, navigating to a non-existent path results in unexpected behavior, often a blank screen or a React Router error.

## Bug
The `App.js` file shows a basic React Router setup missing a route to handle 404 errors. Navigating to a URL that doesn't match any defined routes will result in the default behavior of React Router, which typically isn't user-friendly.

## Solution
The `AppSolution.js` file demonstrates the correct way to handle 404 errors by adding a `Route` with a `path="*"` to catch all unmatched paths. This route renders a custom component, `NotFound`, which provides a more user-friendly experience.

## Setup
1. Clone this repository.
2. Navigate to the project directory:
   `cd react-router-404`
3. Install dependencies:
   `npm install`
4. Run the application:
   `npm start`