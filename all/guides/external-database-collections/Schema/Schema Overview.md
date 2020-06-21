SortOrder: 5
# Schema Overview
The Schema SPI describes the endpoints and payloads for schema API requests to your external database and the payloads for their success and failure responses. Schema API requests may occur whenever your site needs to interact with the data in your external collection. The schema may be cached for at most the amount of time indicated in the `ttl` field of the `schema` object.

