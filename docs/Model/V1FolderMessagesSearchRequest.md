# # V1FolderMessagesSearchRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**since** | **\DateTime** | Only messages received on or after this date (YYYY-MM-DD). |
**before** | **\DateTime** | Only messages received before this date (YYYY-MM-DD). |
**flags** | **string[]** | Only messages carrying all of these IMAP flags, e.g. \\Seen, \\Flagged, \\Answered, $forwarded. |
**uid** | **string** | IMAP UID set: single UID, range (1:100), open range (100:*), or comma-separated list. |
**subject** | **string** | Case-insensitive substring match on the Subject header. OR-combined with from/to/cc/body. |
**from** | **string** | Case-insensitive substring match on the From header. OR-combined with subject/to/cc/body. |
**to** | **string** | Case-insensitive substring match on the To header. OR-combined with subject/from/cc/body. |
**cc** | **string** | Case-insensitive substring match on the Cc header. OR-combined with subject/from/to/body. |
**body** | **string** | Case-insensitive substring match on the message body only (headers excluded). OR-combined with subject/from/to/cc. |
**header** | **string** | Match a specific header as Name:value, e.g. X-Custom-Header:value. Value match is a substring. |
**larger** | **int** | Only messages larger than this size in bytes. |
**smaller** | **int** | Only messages smaller than this size in bytes. |
**text** | **string** | Case-insensitive substring match across headers and body. |

[[Back to Model list]](../../README.md#models) [[Back to API list]](../../README.md#endpoints) [[Back to README]](../../README.md)
