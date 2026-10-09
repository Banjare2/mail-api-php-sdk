# # V1FolderMessagesFlagsBulkRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**uids** | **int[]** | Message UIDs to update. 1-100 entries, each &gt; 0. |
**addFlags** | **string[]** | IMAP flags to set on every listed message, e.g. \\Seen, \\Flagged, \\Answered, $forwarded. |
**removeFlags** | **string[]** | IMAP flags to clear from every listed message. |

[[Back to Model list]](../../README.md#models) [[Back to API list]](../../README.md#endpoints) [[Back to README]](../../README.md)
