# React Native useRef Hook Error with Unmounted Component

This repository demonstrates a common error in React Native when using the `useRef` hook with components that unmount before asynchronous operations within the ref's callback complete.  The example shows how accessing `myRef.current` after the component has unmounted can lead to unexpected behavior or errors.

The `bug.js` file contains the problematic code.  The `bugSolution.js` file provides a solution using a cleanup function in the useEffect hook to prevent this.