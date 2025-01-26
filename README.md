# Express.js 404 Error Handling
This repository demonstrates a common error in Express.js applications where a 404 error is thrown if a requested file is not found using `res.sendFile()`. The solution showcases how to handle this scenario gracefully.
## Bug
The `bug.js` file contains the buggy code. When you run this code and request the `/` route, it will work if `index.html` exists, but will throw a 404 error if the file doesn't exist.
## Solution
The `bugSolution.js` file demonstrates the proper way to handle the error using `fs.existsSync()` to check if the file exists before attempting to send it.