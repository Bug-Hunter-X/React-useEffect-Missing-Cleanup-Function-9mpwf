# React useEffect Missing Cleanup Function
This example demonstrates a common error in React's `useEffect` hook: omitting the cleanup function.  The `useEffect` hook, when used with an empty dependency array (`[]`), is intended to run only once after the initial render.  However, if a cleanup function is not returned, any asynchronous operations or timers started within the effect will not be properly cleaned up when the component unmounts, leading to potential memory leaks or unexpected behavior. 

The provided `bug.js` file contains the buggy code. `bugSolution.js` shows the corrected version.