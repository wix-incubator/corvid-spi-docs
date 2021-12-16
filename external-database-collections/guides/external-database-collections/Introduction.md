SortOrder: 0
# Introduction
Integrate your external database into your Wix site using external collections and building an external database collection adapter.

The External Database Collections SPI describes the API requests your adapter needs to expect from your Wix site, and the responses your Wix site expects in return. The SPI takes the request from your Wix site and converts it into a request that your external database can receive. It also takes the response from the external database and converts it into a JSON response that your Wix site can receive.

You can learn more about working with External Databases on your Wix site [here](https://support.wix.com/en/article/working-with-external-database-collections).

### Mandatory Endpoints
The following endpoints are mandatory and must be implemented in your adapter. All other endpoints are optional.


|Endpoint| Function|
|--------|---------------------------------------------------------|
|Find Schemas| Gets the details of a given list of database tables or collections.|
|List Schemas|  Discover the database tables or collections that are visible to your database user.|
|Get Item |  Get a specific database row or item based on the item's `_id` field.|
|Find Items| Get a list of items based on a filter.|
|Count|  Get the number of rows or items in a table or collection based on a filter.|
|Provision|  Establish the connection between your site and your adapter. |

The implemented endpoints must be exposed via the [schema object](https://www.wix.com/corvid/new-reference/spis/external-database-collections/external-database-collections/schema/schema-object) in the  `allowedOperations` list.

For example:
```json
"schema":
      {
          "displayName": "myCollection",
          "id": "myCollection",
          "allowedOperations": [
              "get",
              "find",
              "count",
              "update",
              "insert",
              "remove"
          ],
          "maxPageSize": 50,
          "ttl": 3600,
          "fields": { "..."}
      }
```


### Data Structures

#### _id
Each table or collection must contain an `_id` column or attribute of type string. 
If you create new data outside of your Wix site, or you are importing new data for use with your site, you must populate this field with a unique value. If you create new data in your site, the Wix Data backend will generate a unique 36-character UUID for each item created.
The `_id` attribute can be any length but if items are created by your Wix site, it must be at least 36 characters long.

#### _owner (optional)
For data created by your Wix site, Wix Data backend will populate the `_owner` attribute with a 36-character UUID identifying the user who created the data. If the visitor is not a logged-in member, the `_owner` attribute is based on a browser cookie and is therefore consistent between sessions. The `_owner` attribute will be null if the new data was created by a backend process.

#### Dates
All dates must be an [ISO](https://en.wikipedia.org/wiki/ISO_8601#Times) string encapsulated in an object.
     For example: "myDate" :{“$date”:”2001-02-11T00\:00\:00.000Z”}
