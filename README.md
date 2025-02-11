# Silent Failure on router.push to undefined route in Next.js

This repository demonstrates a subtle bug in Next.js where using `router.push` with an undefined route results in a silent failure—no errors or warnings are thrown. This can be extremely difficult to track down, especially during development.

## The Bug
The provided `bug.js` file contains a component that attempts to navigate to a route that doesn't exist using `router.push('/not-defined-route')`.  This action doesn't produce any errors or warnings in Next.js, making it challenging to detect during development.

## The Solution
The solution provided in `bugSolution.js` demonstrates how to address this by adding a check for the route's existence before attempting navigation. This approach ensures a more robust and reliable user experience. 