---
description: >-
  This article provides an overview of the rate limiting policies within the
  platform to show how many requests a tenant can sustain.
---

# Rate limiting Policies

#### How Rate Limiting Works

By default, each tenant is limited to **3,000 requests per minute**. This limit is set to balance high-demand usage with overall system performance. The API will return an HTTP 429 Too Many Requests status code if a tenant exceeds this limit.

#### Rate Limit Headers

To manage your API usage effectively, the response headers include the following rate limit information:

* **X-RateLimit-Limit**: This indicates the maximum number of requests your tenant is allowed per minute (3,000 by default).
* **X-RateLimit-Remaining**: Shows the number of requests remaining within the current time window.
* **X-RateLimit-Reset**: Provides the time (in Unix epoch format) when the rate limit will reset, allowing you to resume making requests.

**Example Response Headers:**

```http
X-RateLimit-Limit: 3000
X-RateLimit-Remaining: 450
X-RateLimit-Reset: 1632425760
```

#### Exceeding the Limit

If your tenant exceeds the allowed request limit, the API will respond with an **HTTP 429 Too Many Requests** status code. The response will include the rate limit headers, helping you understand when the limit will reset and when you can resume making requests.

**Example Response:**

```http
HTTP/1.1 429 Too Many Requests
X-RateLimit-Limit: 3000
X-RateLimit-Remaining: 0
X-RateLimit-Reset: 1632425760
```

#### Best Practices for Managing Rate Limits

To avoid hitting the rate limit and ensure smooth API usage, follow these best practices:

* **Implement Retry Logic**: If you encounter an HTTP 429 response, use the `X-RateLimit-Reset` Header to determine when you can safely retry your requests. Based on the reset time, implement a retry mechanism with an appropriate delay.

For information on requesting a higher service quota, please refer to our [#request-additional-service-quota](./#request-additional-service-quota "mention") section.
