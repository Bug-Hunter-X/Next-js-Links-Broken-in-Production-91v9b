# Next.js Links Broken in Production

This repository demonstrates a common issue in Next.js applications where links work perfectly in development but fail in production.  The problem arises from misconfiguration of the `basePath` or incorrect usage of relative paths within `Link` components.

## Bug

The `bug.js` file shows a simple Next.js component with links to the `/` (home) and `/about` routes.  In production, these links will result in 404 errors, even if the routes exist.

## Solution

The `bugSolution.js` file provides a corrected version that addresses the potential issues, explaining how to ensure proper linking in production.  This solution may involve ensuring the `basePath` is correctly set in your Next.js configuration or using absolute paths for the links.