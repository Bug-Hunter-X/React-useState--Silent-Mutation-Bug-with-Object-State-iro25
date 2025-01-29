# React useState Silent Mutation Bug

This repository demonstrates a common, yet subtle, bug in React applications involving the `useState` hook and object state.  Directly modifying object properties within the state leads to unexpected behavior where the component fails to re-render, causing the UI to become stale.

The `bug.js` file shows the problematic code. The `bugSolution.js` file provides a corrected version that utilizes the functional update pattern to resolve the issue.

## How to reproduce

1. Clone this repository.
2. Navigate to the repository directory.
3. Run `npm install` to install the dependencies.
4. Run `npm start` to start the development server.
5. Observe the counter; clicking "Increment" will not increment the count, demonstrating the bug.

## Solution

Refer to `bugSolution.js` for a correct implementation that uses a functional update pattern to ensure proper re-rendering.