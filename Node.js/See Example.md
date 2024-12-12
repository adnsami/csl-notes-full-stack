```js
// successful response
{
	status: 200,
	success: true,
	data: [{...}, {...}],
	error: null
}

// error response
{
	status: 401,
	success: false,
	data: null,
	error: {
		// VALIDATION_ERROR | RESOURCE_NOT_FOUND | RATE_LIMIT_EXCEEDED
		type: 'UNAUTHORIZED', 
        message: "Authentication required",
        details: "No valid access token provided",
	}
}
```