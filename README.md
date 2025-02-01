# React useEffect Hook Runs on Every Render

This repository demonstrates a common error in React where the `useEffect` hook runs on every render due to a missing dependency array.  This can lead to performance issues and unexpected behavior.

## Problem

The `useEffect` hook in the provided `bug.js` file lacks a dependency array.  As a result, the effect runs after every render, causing the console log statement to execute repeatedly and potentially impacting performance.

## Solution

The `bugSolution.js` file demonstrates the correct usage.  By adding `[count]` as the dependency array, the effect only runs when the value of `count` changes.