# Rate Limits

In order to prevent abuse of the API there are rate limits on all API endpoints. Currently rate limits are global across
all requests and can dynamically change. In order to accommodate for this, the client must use the rate limit headers
returned whenever a request is made.

## Rate Limit Headers

Currently there are three rate limit headers.

`x-ratelimit-limit` - Total amount of requests allowed

`x-ratelimit-remaining` - Amount of requests left

`x-ratelimit-reset` - Unix Epoch time when amount of requests resets to the total

## Exceeding Rate Limits

If the client exceeds a rate limit the API will return HTTP code 429 with a message in data stating
`You are being rate limited`.

> ℹ This response will soon be improved to better handle exceeding a rate limit.