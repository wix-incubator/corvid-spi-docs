SortOrder: 1
# Authentication

The External Database Collections SPI uses the `request context object` to manage authentication and authorization. HTTP authentication is not implemented. The `settings` object within the request context object contains the `secretKey` for authentication purposes. This key is configured in the Wix Editor when [adding the external collection](https://support.wix.com/en/article/corvid-adding-and-deleting-an-external-database-collection) and send by the Wix Data backend in every request.

In addition to the the settings object, the request context object contains the `instanceId`,`installationId`, `memberId`, and `memberRole`. Each of these properties can be used to implement a permissions model controlling access to operations and data. Permissions can be implemented based on the site making the of the request, the external collection within the site, the visitor's member ID and the member's role.

[Learn more](www.wix.com) about the `request context object`.
