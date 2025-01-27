# React useEffect Infinite Loop Bug
This repository demonstrates a common React bug involving the `useEffect` hook and its dependency array.  The bug causes an infinite rendering loop due to an improperly configured dependency array.

## The Problem
The `useEffect` hook, when used incorrectly, can create a situation where it continuously updates the state, triggering re-renders, and leading to an infinite loop.

## The Solution
To prevent this, ensure that the dependency array includes all values from the component's state that the `useEffect` depends upon.  In this case, the `count` variable must be included in the dependency array.

## How to Reproduce
1. Clone this repository.
2. Run `npm install`.
3. Run `npm start`.
4. Observe the console output and the infinite loop behavior.
5. Uncomment the corrected `useEffect` dependency array in `bugSolution.js` to see how it fixes the problem.