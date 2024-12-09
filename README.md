# Unexpected Client-Side Navigation Behavior in Next.js 15 App Router

This repository demonstrates a potential issue with client-side navigation in Next.js 15's App Router.  The bug involves unexpected rendering or routing issues when using `next/link` with certain navigation scenarios.  The solution provides a method to mitigate this problem.

## Bug

The bug is demonstrated in `bug.js`. Client side navigation using `next/link` might result in a broken navigation or the page not rendering correctly depending on the route and its loading behaviour.

## Solution

The solution is provided in `bugSolution.js`. This addresses the issue by explicitly handling the potential race condition that the bug highlights. It uses better navigation methods, or more robust state management, or a different approach to ensure the rendering is correct across different navigation scenarios.

## Setup

1. Clone this repository.
2. Run `npm install` to install dependencies.
3. Run `npm run dev` to start the development server.

Navigate between the routes to reproduce the error and observe the fix.