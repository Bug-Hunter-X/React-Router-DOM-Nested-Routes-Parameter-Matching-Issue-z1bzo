# React Router DOM Nested Route Parameter Matching Issue

This repository demonstrates a common issue when using nested routes with parameters in React Router DOM.  The problem arises when a route with parameters is nested under a route without parameters. In this specific case, the route `/:id` will never match because the parent route (`/`) will always match first. This prevents the `User` component from ever rendering.

## Solution
The solution involves re-organizing the routes to address the routing conflict. See `bugSolution.js` for the fix.