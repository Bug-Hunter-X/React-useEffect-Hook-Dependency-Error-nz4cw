# React UseEffect Dependency Issue
This example demonstrates a common error in React's `useEffect` hook: an incorrectly used dependency array.
The `useEffect` hook is intended to perform side effects based on changes in specified dependencies. However, the provided code has an error in its conditional logic, leading to unintended side effects.
## Problem
The `useEffect` hook's conditional statement `if (count)` will always execute when `count` is greater than 0, but it should only run when the count changes.  This results in unnecessary re-renders and side-effects. 
## Solution
The solution involves refining the useEffect dependency array.  It should only run when count changes, which is already handled correctly because count is in the dependency array. The solution also simplifies the logic by removing the unnecessary conditional statement.