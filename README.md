# React useEffect Infinite Loop Bug

This repository demonstrates a common React bug involving the `useEffect` hook and its dependency array.  The bug causes an infinite render loop, flooding the console with logs.

The problem lies in the incorrect definition of the dependency array for `useEffect`.  Without including `count` in the dependency array, the effect runs after every render, leading to the count incrementing, triggering another render, and continuing the loop.

The solution involves correctly specifying `count` as a dependency, so the effect only runs when `count` changes.

## Setup

Clone this repository and run `npm install` to install the necessary dependencies.

## Run

Run `npm start` to start the development server and observe the bug in action.

Then, examine the `bugSolution.js` file to see the corrected code.