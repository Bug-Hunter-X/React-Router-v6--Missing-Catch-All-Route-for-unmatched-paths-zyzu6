# React Router v6: Missing Catch-All Route

This example demonstrates a common issue in React Router v6 where unexpected behavior occurs when no defined route matches the current URL.  Without a catch-all route (`/*`), the application might display nothing or throw an error, depending on the configuration.

## Problem

The `App` component uses `react-router-dom` to define routes.  However, it fails to include a route to handle cases when none of the explicit paths match.  If the user navigates to a URL not specified in `Routes` (e.g., `/invalid-path`), the application won't render anything correctly.

## Solution

Add a catch-all route to handle any unmatched URL paths. This prevents unexpected behavior or errors.