# Hostinger\FeedbackApi

All URIs are relative to https://api.mail.hostinger.com, except if the operation defines another base path.

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**submitFeedback()**](FeedbackApi.md#submitFeedback) | **POST** /api/v1/mailboxes/{mailboxResourceId}/feedback | Submit feedback |


## `submitFeedback()`

```php
submitFeedback($mailboxResourceId, $v1FeedbackSubmitRequest)
```

Submit feedback

Report a problem or suggestion about this API or the MCP server to the Hostinger mail team.  Report when a call returned 4xx/5xx or unexpected data, was too slow, when documentation was missing or unclear, or when a capability you needed does not exist. Mention the failing operation and the status code you received so the team can find the request. Never include tokens, passwords or email contents: the message is scrubbed of secrets and capped at 2000 characters. Send one report per distinct issue.  A `429` (`ERR_FEEDBACK_RATE_LIMIT`) means feedback for this customer was submitted less than ten seconds ago; wait and retry.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer authorization: BearerAuth
$config = Hostinger\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new Hostinger\Api\FeedbackApi(config: $config);
$mailboxResourceId = AC1a2b3c4d5e6f7g; // string | Resource ID of the managed mailbox the feedback is about, as returned by `GET /api/v1/me`.
$v1FeedbackSubmitRequest = new \Hostinger\Model\V1FeedbackSubmitRequest(); // \Hostinger\Model\V1FeedbackSubmitRequest

try {
    $apiInstance->submitFeedback($mailboxResourceId, $v1FeedbackSubmitRequest);
} catch (Exception $e) {
    echo 'Exception when calling FeedbackApi->submitFeedback: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **mailboxResourceId** | **string**| Resource ID of the managed mailbox the feedback is about, as returned by &#x60;GET /api/v1/me&#x60;. | |
| **v1FeedbackSubmitRequest** | [**\Hostinger\Model\V1FeedbackSubmitRequest**](../Model/V1FeedbackSubmitRequest.md)|  | |

### Return type

void (empty response body)

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)
