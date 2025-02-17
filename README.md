# React useEffect Infinite Loop Bug

This repository demonstrates a common error in React's `useEffect` hook:  omitting the dependency array. This leads to an infinite render loop, significantly impacting performance and potentially crashing the browser.

## Bug

The `bug.js` file contains a component with a `useEffect` hook that lacks a dependency array. The effect runs on every render, causing an infinite loop of log messages and re-renders.

## Solution

The `bugSolution.js` file corrects this by adding the `count` variable to the dependency array.  The effect now only runs when `count` changes, resolving the infinite loop.