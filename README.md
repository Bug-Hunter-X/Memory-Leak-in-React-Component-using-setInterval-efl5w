# React setInterval Memory Leak
This example demonstrates a common memory leak in React components when using `setInterval` within the `useEffect` hook without proper cleanup.
The `setInterval` function continues to run even after the component unmounts, causing a memory leak.
The solution shows how to fix this by returning a cleanup function from the `useEffect` hook.