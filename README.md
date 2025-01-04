# React useEffect Bug

This repository demonstrates a common misunderstanding of the `useEffect` hook in React 18 and 19.  The bug arises from an incorrect understanding of how the dependency array works.  The solution shows how to correctly use the dependency array to control when the effect runs.

## Bug
The initial implementation of `MyComponent` unintentionally causes the `useEffect` to run after every render, which may not be the intended behavior.

## Solution
The solution correctly adds `count` to the dependency array, which correctly limits the effect's execution to state updates.
