# React Native useCallback Infinite Loop Bug

This repository demonstrates a common bug in React Native applications where using the `useCallback` hook with a function that internally uses `useState` results in an infinite loop. The issue is caused by the changing closure of the inner function, triggering unnecessary re-renders.

The `bug.js` file showcases the problematic code. The `bugSolution.js` file provides a corrected implementation that resolves this issue.  The key is to properly manage dependencies within `useCallback` to prevent unnecessary function recreations.