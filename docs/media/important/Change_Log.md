# Change Log

## Removal of uniform data structure and ISO creation times

### TBD

* The data structure that was returned by all API endpoints will no longer be present in favor of only returning the data.
* All objects returned by the API will no longer contain ISO-8601 `created_at` fields in favor of parsing the snowflake ID for an instantaneous timestamp.
* `quickURL` (in QuickLinks) has been renamed to `quick_url` to conform with the rest of the API.
* `url` (in QuickLinks) has been renamed to `redirect_url` for clarity.
