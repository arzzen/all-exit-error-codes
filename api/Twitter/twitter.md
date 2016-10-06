# Twitter API Error Codes

This list comes directly from [Twitter's Pulic API response codes page](https://dev.twitter.com/overview/api/response-codes).

#### HTTP Status Codes
The Twitter API attempts to return appropriate HTTP status codes for every request

| HTTP Error Code  | Text    | Description  |
| :-------------: |:-------------| ------------|
| 200 | OK | Succes.  **Not an error code** |
| 304 | 304 | There was no new data to return.  **Not an error code** |
| 400 | Bad Request | The request was invalid or cannot be otherwise served. An accompanying error message will explain further. In API v1.1, requests without authentication are considered invalid and will yield this response. |
| 401 | Unauthorized | [Authentication credentials](https://dev.twitter.com/oauth) were missing or incorrect. Also returned in other circumstances, for example all calls to API v1 endpoints now return 401 (use [API v1.1](https://dev.twitter.com/rest/public) instead). |
| 403 | Forbidden | The request is understood, but it has been refused or access is not allowed. An accompanying error message will explain why. This code is used when requests are being denied due to [update limits](https://support.twitter.com/articles/15364-about-twitter-limits-update-api-dm-and-following). Other reasons for this status being returned are listed alongside the response codes in the table below. |
| 404 | Not Found | The URI requested is invalid or the resource requested, such as a user, does not exists. Also returned when the requested format is not supported by the requested method. |
| 406 | Not Acceptable | Returned by the Search API when an invalid format is specified in the request. |
| 410 | Gone | This resource is gone. Used to indicate that an API endpoint has been turned off. For example: “The Twitter REST API v1 will soon stop functioning. Please migrate to API v1.1.” |
| 420 | Enhance Your Calm | Returned by the version 1 Search and Trends APIs when [you are being rate limited](https://dev.twitter.com/rest/public/rate-limiting). |
| 422 | Unprocessable Entity | Returned when an image uploaded to [POST account / update_profile_banner](https://dev.twitter.com/rest/reference/post/account/update_profile_banner) is unable to be processed. |
| 429 | Too Many Requests | Returned in API v1.1 when a request cannot be served due to the application’s rate limit having been exhausted for the resource. See [Rate Limiting in API v1.1](https://dev.twitter.com/rest/public/rate-limiting). |
| 500 | Internal Server Error | Something is broken. Please post [to the developer forums](https://twittercommunity.com/) so the Twitter team can investigate. |
| 502 | Bad Gateway	 | Twitter is down or being upgraded. **Not your fault**|
| 503 | Service Unavailable | The Twitter servers are up, but overloaded with requests. Try again later. **Not your fault**|
| 504 | Gateway timeout | The Twitter servers are up, but the request couldn’t be serviced due to some failure within our stack. Try again later. **Not your fault** |
