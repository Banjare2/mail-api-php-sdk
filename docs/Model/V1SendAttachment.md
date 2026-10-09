# # V1SendAttachment

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**filename** | **string** | File name shown to the recipient, including extension. |
**content** | **string** | Attachment body. Base64-encoded by default; set encoding to switch. |
**contentType** | **string** | MIME type of the attachment, e.g. application/pdf. Not inferred from filename; set it explicitly so clients render the attachment correctly. |
**cid** | **string** | Content-ID for inline images. Reference from HTML as &lt;img src&#x3D;\&quot;cid:logo\&quot;&gt;. |
**encoding** | **string** | Encoding of content. Defaults to base64. |

[[Back to Model list]](../../README.md#models) [[Back to API list]](../../README.md#endpoints) [[Back to README]](../../README.md)
