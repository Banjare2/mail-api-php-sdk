# # V1WebhooksCreateRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **string** | Human-readable webhook name. |
**description** | **string** | Optional free-text note about the webhook purpose. |
**events** | **string[]** | Event types that trigger a delivery. |
**status** | **string** | Initial delivery state. Only active webhooks receive events. | [default to 'active']
**url** | **string** | HTTPS endpoint that receives POST deliveries, authenticated with the webhook secret as &#x60;Authorization: Bearer &lt;secret&gt;&#x60;. Must be a public domain name (no IPs or internal hosts). |

[[Back to Model list]](../../README.md#models) [[Back to API list]](../../README.md#endpoints) [[Back to README]](../../README.md)
