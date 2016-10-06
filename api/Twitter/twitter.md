# Twitter API Error Codes

This list comes directly from [Twitter's Pulic API response codes page](https://dev.twitter.com/overview/api/response-codes).

## HTTP Status Codes
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
| 502 | Bad Gateway | Twitter is down or being upgraded. **Not your fault**|
| 503 | Service Unavailable | The Twitter servers are up, but overloaded with requests. Try again later. **Not your fault**|
| 504 | Gateway timeout | The Twitter servers are up, but the request couldn’t be serviced due to some failure within our stack. Try again later. **Not your fault** |

## Error Messages and Codes
When the Twitter API returns error messages, it does so in JSON format. For example, an error might look like this:
```js
{"errors":[{"message":"Sorry, that page does not exist","code":34}]}
```

### Error Codes
In addition to descriptive error text, error messages contain machine-parseable codes. While the **text for an error message may change, the codes will stay the same**.

| Code | Text | Description |
| :---------------------: |:-------------| ------------|
| 32 | Could not authenticate you | Your call could not be completed as dialed.|
| 34 | Sorry, that page does not exist | Corresponds with an HTTP 404 - the specified resource was not found.|
| 64 | Your account is suspended and is not permitted to access this feature | Corresponds with an HTTP 403 — the access token being used belongs to a suspended user and they can’t complete the action you’re trying to take. |
| 68 | The Twitter REST API v1 is no longer active. Please migrate to API v1.1. https://dev.twitter.com/rest/public | Corresponds to a HTTP request to a retired v1-era URL.|
| 88 | Rate limit exceeded | The request limit for this resource has been reached for the current rate limit window.|
| 89 | Invalid or expired token | The access token used in the request is incorrect or has expired. Used in API v1.1|
| 92 | SSL is required | Only SSL connections are allowed in the API, you should update your request to a secure connection. See [how to connect using SSL](https://dev.twitter.com/overview/api/ssl)|
| 130 | Over capacity | Corresponds with an HTTP 503 - Twitter is temporarily over capacity.|
| 131 | Internal error | Corresponds with an HTTP 500 - An unknown internal error occurred.|
| 135 | Could not authenticate you | Corresponds with a HTTP 401 - Your oauth_timestamp is either ahead or behind our acceptable range.|
| 136 | You have been blocked from {action} | Corresponds with a HTTP 401 - The user associated with the action you are performing has blocked you.|
| 161 | You are unable to follow more people at this time | Corresponds with HTTP 403 — thrown when a user cannot follow another user due to some kind of limit.|
| 179 | Sorry, you are not authorized to see this status | Corresponds with HTTP 403 — thrown when a Tweet cannot be viewed by the authenticating user, usually due to the tweet’s author having protected their tweets.|
| 185 | User is over daily status update limit | Corresponds with HTTP 403 — thrown when a tweet cannot be posted due to the user having no allowance remaining to post. Despite the text in the error message indicating that this error is only thrown when a daily limit is reached, this error will be thrown whenever a posting limitation has been reached. Posting allowances have roaming windows of time of unspecified duration.|
| 187 | Status is a duplicate | The status text has been Tweeted already by the authenticated account.|
| 215 | Bad authentication data	| Typically sent with 1.1 responses with HTTP code 400. The method requires authentication but it was not presented or was wholly invalid.|
| 226 | This request looks like it might be automated. To protect our users from spam and other malicious activity, we can’t complete this action right now. | We constantly monitor and adjust our filters to block spam and malicious activity on the Twitter platform. These systems are tuned in real-time. If you get this response our systems have flagged the Tweet or DM as possibly fitting this profile. If you feel that the Tweet or DM you attempted to create was flagged in error, please report the details around that to us by filing a ticket at [https://support.twitter.com/forms/platform](https://support.twitter.com/forms/platform).|
| 231 | User must verify login | Returned as a challenge in [xAuth](https://dev.twitter.com/oauth/xauth) when the user has [login verification](https://dev.twitter.com/oauth/xauth#2fa) enabled on their account and needs to be directed to twitter.com to [generate a temporary password](https://twitter.com/settings/applications).|
| 251 | This endpoint has been retired and should not be used. | Corresponds to a HTTP request to a retired URL.|
| 261 | Application cannot perform write actions. | Corresponds with HTTP 403 — thrown when the application is restricted from POST, PUT, or DELETE actions. See [How to appeal application suspension and other disciplinary actions](https://support.twitter.com/articles/72585).|
| 271 | You can’t mute yourself. | Corresponds with HTTP 403. The authenticated user account cannot mute itself.|
| 272 | You are not muting the specified user. | Corresponds with HTTP 403. The authenticated user account is not muting the account a call is attempting to unmute.|
| 354 | The text of your direct message is over the max character limit. | Corresponds with HTTP 403. The message size exceeds the number of characters permitted in a direct message.|
