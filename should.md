Mime type definitions are spread across several resources. The mime type definitions should be in compliance with [RFC 6838](http://tools.ietf.org/html/rfc6838).
<a name="operationSummary"></a>summary | `string` | A short summary of what the operation does. 
For maximum readability in the swagger-ui, this field SHOULD be less than 120 characters.
<a name="responseSchema"></a>schema | [Schema Object](#schemaObject) | A definition of the response structure. It can be a primitive, an array or an object. If this field does not exist, it means no content is returned as part of the response. 
As an extension to the [Schema Object](#schemaObject), its root `type` value may also be `"file"`. This SHOULD be accompanied by a relevant `produces` mime-type.
<a name="exampleMimeType"></a>{[mime type](#mimeTypes)} | Any | The name of the property MUST be one of the Operation `produces` values (either implicit or inherited). The value SHOULD be an example of what such a response would look like. 
When using arrays, XML element names are *not* inferred (for singular/plural forms) and the `name` property should be used to add that information. See examples for expected behavior.
<a name="xmlNamespace"></a>namespace | `string` | The URL of the namespace definition. Value SHOULD be in the form of a URL.
<a name="securitySchemeAuthorizationUrl"></a>authorizationUrl | `string` | `oauth2` (`"implicit"`, `"accessCode"`) | **Required.** The authorization URL to be used for this flow. This SHOULD be in the form of a URL.
<a name="securitySchemeTokenUrl"></a>tokenUrl | `string` | `oauth2` (`"password"`, `"application"`, `"accessCode"`) | **Required.** The token URL to be used for this flow. This SHOULD be in the form of a URL.
