# React Router v6 Catch-All Route Conflict

This repository demonstrates a common issue encountered when using the catch-all route (`/*`) in React Router v6.  The catch-all route unintentionally intercepts routes that should be handled by other more specific routes.

The problem stems from the order of routes.  If a catch-all route is placed before more specific routes, it will always match first, preventing other routes from being reached.

The solution involves carefully ordering routes within the `Routes` component, placing the catch-all route last.