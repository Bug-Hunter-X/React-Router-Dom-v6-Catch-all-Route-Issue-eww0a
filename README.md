# React Router Dom v6 Catch-all Route Issue

This repository demonstrates a common issue encountered when using the catch-all route (`/*`) in React Router Dom v6. The catch-all route, intended to handle routes not explicitly defined, can unexpectedly interfere with nested routes. This leads to rendering issues and prevents other routes from working as expected.

## Problem Description

The problem arises from the order in which React Router v6 matches routes. The catch-all route, due to its nature, matches any path.  If placed before other routes, it will always take precedence. This can break nested routing or routes with dynamic segments.