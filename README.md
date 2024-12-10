# Express.js Route Handler Missing JSON Response for 404 Error

This repository demonstrates a common error in Express.js route handlers: failing to send a JSON response, specifically when handling a 404 (Not Found) error.  The bug causes the server to return a plain text error message, which can break client-side applications expecting a JSON response.

The `bug.js` file shows the erroneous code, and `bugSolution.js` provides the corrected version.

## Bug
The primary issue is that the error response doesn't send a proper JSON object.  The solution properly formats the response for better interoperability with clients.