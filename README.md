# React useEffect Infinite Rendering Bug

This repository demonstrates a common bug in React applications related to the `useEffect` hook and its dependency array. The `MyComponent` component renders infinitely due to an incorrect dependency array in the `useEffect` hook.

## Bug Description

The bug occurs because the `count` variable is not included in the dependency array of the `useEffect` hook. This causes the effect to run on every render, leading to an infinite loop.  The `console.log` statement helps illustrate this.

## Bug Solution

The solution involves adding `count` to the dependency array.  This ensures the effect only runs when the `count` variable changes.