# React useEffect Hook Missing Return Statement

This repository demonstrates a common yet easily overlooked bug in React applications: forgetting the return statement within a `useEffect` hook.  This can lead to memory leaks and unexpected behavior.

## Bug Description

The `useEffect` hook in the `bug.js` file is missing a return statement.  This is problematic because the code within the `useEffect` will run on mount, but also continuously if not returned to cleanup.