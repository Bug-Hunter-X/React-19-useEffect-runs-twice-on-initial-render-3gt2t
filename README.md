# React 19 useEffect runs twice on initial render

This repository demonstrates a common issue in React 19 where the useEffect hook runs twice on the initial render of a functional component.  The problem is identified and a solution is provided.

## Problem

The `useEffect` hook, intended to perform side effects after component rendering, is unexpectedly executing twice during the initial mount. This can lead to unintended consequences and performance issues. 

## Solution

The solution involves correctly specifying the dependencies array in the `useEffect` hook.  Ensure that the array includes all values from the component's scope that the effect relies upon.