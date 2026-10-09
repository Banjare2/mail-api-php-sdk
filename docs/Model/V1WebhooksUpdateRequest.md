# # V1WebhooksUpdateRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **string** | Human-readable webhook name. |
**description** | **string** | Free-text note about the webhook purpose. Send null to clear. |
**events** | **string[]** | Event types that trigger a delivery. Replaces the current list. |
**status** | **string** | Delivery state. Only active webhooks receive events; paused keeps config but stops deliveries. |
**url** | **string** | HTTPS endpoint that receives POST deliveries, authenticated with the webhook secret as &#x60;Authorization: Bearer &lt;secret&gt;&#x60;. Must be a public domain name (no IPs or internal hosts). |

[[Back to Model list]](../../README.md#models) [[Back to API list]](../../README.md#endpoints) [[Back to README]](../../README.md)
