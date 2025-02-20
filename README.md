# React useEffect Infinite Loop Bug

This repository demonstrates a common error in React's `useEffect` hook: an infinite loop caused by missing dependencies.

## The Bug
The `bug.js` file contains a `MyComponent` that uses `useEffect` without specifying any dependencies. This causes the effect to run after every render, leading to an infinite loop of re-renders and console logs.

## The Solution
The `bugSolution.js` file shows the corrected component.  By adding `count` as a dependency, the effect now only runs when `count` changes, fixing the infinite loop.

## How to Reproduce
1. Clone this repository.
2. Run `npm install` to install dependencies.
3. Run `npm start` to start the development server.
4. Observe the console logs and the component's behavior.