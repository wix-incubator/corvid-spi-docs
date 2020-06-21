SortOrder: 1
# Authentication

The External Database Collections SPI uses the [request context object](https://www.wix.com/corvid/new-reference/spis/external-database-collections/external-database-collections/request-context/request-context-object) to manage authentication and authorization. HTTP authentication is not implemented. The `settings` object within the request context object can contain a key for authentication purposes. In the prototype and examples, the `secretKey` property is used. This key is configured in the Wix Editor when [adding the external collection](https://support.wix.com/en/article/corvid-adding-and-deleting-an-external-database-collection) and sent by the Wix Data backend in every request.

In addition to the settings object, the request context object contains the `instanceId`,`installationId`, `memberId`, and `memberRole`. Each of these properties can be used to implement a permissions model controlling access to operations and data. Permissions can be implemented based on the site making the request, the external collection within the site, the visitor's member ID, and the member's role.

